# Nginx
### ansible-role-nginx
This role installs Nginx along with config files. 

Default config files will be installed by the role if the following variables are not defined in the playbook.

## Required Variables

group_vars/dev.yml
```bash
nginx_conf: group_files/<hostgroup>/nginx/nginx.conf
nginx_confd_directory: group_files/<hostgroup>/nginx/conf.d
nginx_sites_directory: group_files/<hostgroup>/nginx/sites_available
nginx_ssl_keys:
nginx_ssl_crts:
```

## Files & Templates
All Nginx config files should be located in the directories stated by the above variables

## Author

rwhite@globeandmail.com | tlannder@globeandmail.com
