# Nginx
### ansible-role-nginx
This role installs Nginx along with config files. 

Default config files will be installed by the role if the following variables are not defined in the playbook.

## Required Variables
The following variables are required to customize the Nginx install. The variables should point to the location of the customized files.

For example, 

group_vars/dev.yml
```bash
nginx_conf: group_files/<hostgroup>/nginx/nginx.conf
nginx_confd_dir: group_files/<hostgroup>/nginx/conf.d
nginx_sites_dir: group_files/<hostgroup>/nginx/sites-available
nginx_ssl_keys: group_files/<hostgroup>/nginx/ssl/key/
nginx_ssl_crts: group_files/<hostgroup>/nginx/ssl/crt/
```

## Files & Templates
All Nginx config files should be located in the directories stated by the above variables.  When nginx_conf, nginx_confd_dir and nginx_sites_dir are not defined, default values set within the role are used.  

## Author

rwhite@globeandmail.com | tlannder@globeandmail.com
