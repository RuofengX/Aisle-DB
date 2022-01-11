# Aisle-DB  
Use docker-compose and mount nfs in container to run a mysql8 db.  

## Spec
1. Use mysql_native_password as default default_authentication_plugin, which increases compatibility with `mysql5.7`.  
2. Mount a NFS file system at /mnt/db-data as datadir.  
3. Allow container to use SYS_NICE capacity, which is needed by a new feature called resource pool in mysql8.  