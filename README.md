Role Name
=========

This role takes backup of a filesystem and restores it, further uploads backup to S3 bucket

Assumptiom
------------

Aws Cli is pre-installed on the server where filesystem is present

Role Variables
--------------

source_file: "/tmp/backup"

backup_file: "/opt/backup"

backup_dir: "/opt/"

s3_bucket_name: "backupFile"

backup_only: true

restore_only: false

Here when only backup is needs to be done set backup_only as "true" and restore_only as "false" and for restore only backup_only as "false" and 
restore_only as "false"

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: backup_hosts
      roles:
         - { role: sandy724.FileSystemBackupRestore }

License
-------

BSD

Author Information
------------------

www.opstree.com

blog.opstree.com	
