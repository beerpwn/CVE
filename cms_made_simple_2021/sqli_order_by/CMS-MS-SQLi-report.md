## SQL injection

### Author: Riccardo Krauter @ [Soter IT Security](https://soteritsecurity.com) <img src="https://soteritsecurity.com/img/favicon.png" width="20">

The vulnerability is located in the `modules/News/function.admin_articlestab.php` file.

![alt img](sca_1.PNG)

![alt img](sca_2.PNG)

The `sortby` parameter is sanitized by replacing the `'` with the `_` character. As it is possible to notice the `$sortby` variable is concatenated with `$query1`, but it is possible to inject arbitrary SQL language without using the `'`.
As proof of concept, please consider the following screen-shot

![alt img](sqli_poc.PNG)

Notice that the server will sleep for 4 seconds since the query has two results (row).

* time based payload payload: `(SELECT (CASE WHEN 1=1 THEN sleep(2) ELSE news_id END)) -- `
