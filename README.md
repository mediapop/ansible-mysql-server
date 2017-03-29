MySQL Server
============

MySQL 5.7 preconfigured for the web with emoji and timezone support. Specifically we set:

```ini
character_set_server = utf8mb4
collation_server = utf8mb4_unicode_ci
innodb_large_prefix = on
innodb_file_format = BARRACUDA
innodb_default_row_format = DYNAMIC
```

Requirements
------------

This role requires Ansible 2.0 or higher. You **must** set `mysql_root_db_pass`.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows:

```yml
mysql_port: 3306
mysql_bind_address: "0.0.0.0"
mysql_root_db_pass: asdf1234
performance_schema: ON
mysql_sql_mode: "ONLY_FULL_GROUP_BY,STRICT_TRANS_TABLES,NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_AUTO_CREATE_USER,NO_ENGINE_SUBSTITUTION"
```

License
-------

MIT

Author Information
------------------

[Media Pop](http://www.mediapop.co)
