# ansible pastir.postgresql

1. Default installation version PostgreSQL 17

2. Packages are installed by default:

* postgresql-client-17
* postgresql-17
* postgresql-doc-17
* libpq-dev


Example:  postgresql_install.yml
 ```
 - name: install postgresql
   hosts: pghost
   vars:
     postgresql_version: 16
     postgresql_packages:
       - postgresql-client-16
       - postgresql-16
       - libpq-dev
       
   roles:
     - role: pastir.postgresql
 
 ```
