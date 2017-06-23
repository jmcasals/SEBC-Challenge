$cat /etc/yum.repos.d/MariaDB.repo

# MariaDB 10.2 RedHat repository list - created 2017-06-06 14:25 UTC
# http://downloads.mariadb.org/mariadb/repositories/

[mariadb]
name = MariaDB
baseurl = http://yum.mariadb.org/5.5/rhel7-ppc64/
gpgkey=https://yum.mariadb.org/RPM-GPG-KEY-MariaDB
gpgcheck=1


 SHOW VARIABLES like "%hostname%";
+---------------+--------------------------------------------+
| Variable_name | Value                                      |
+---------------+--------------------------------------------+
| hostname      | ip-172-31-39-89.eu-west-1.compute.internal |
+---------------+--------------------------------------------+
1 row in set (0.00 sec)



 SHOW VARIABLES like "%version%";
+-------------------------+---------------------+
| Variable_name           | Value               |
+-------------------------+---------------------+
| innodb_version          | 5.5.49-MariaDB-38.0 |
| protocol_version        | 10                  |
| slave_type_conversions  |                     |
| version                 | 5.5.52-MariaDB      |
| version_comment         | MariaDB Server      |
| version_compile_machine | x86_64              |
| version_compile_os      | Linux               |
+-------------------------+---------------------+
7 rows in set (0.00 sec)


 SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
9 rows in set (0.00 sec)


