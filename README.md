# midih
## MIDIH collaboration platform

The docker-compose.yml file can be used to start the MIDIH Platform. 

In order to use it, it is necessary to set and export the following environment variables to reflect the docker host specific configuration.
```shell
DIH_PORTAL_NAME = <portal_FQDN> | <portal_ipaddr:portal_port> | <host_ip:portal_port>
PORTAL_WEB_PORT = <docker_published_portal_web_port>
PORTAL_AJP_PORT = <docker_published_portal_ajp_port>
GOOGLE_ANALYTICS_KEY = <google key for portal analytics>

DIH_IDM_NAME = <idm_FQDN> | <idm_ipaddr:idm_port> | <host_ip:idm_port>
IDM_WEB_PORT = <docker_published_idm_web_port>

DIH_MKPL_NAME = <mkpl_FQDN> | <mkpl_ipaddr:mkpl_port> | <host_ip:mkpl_port>
MKPL_WEB_PORT = <docker_published_mkpl_web_port>
MKPL_ADMIN_EMAIL = <mkpl_admin_email_address>
MKPL_EMAIL_USER = <mkpl_admin_email_user>
MKPL_EMAIL_PASSWD = <mkpl_admin_email_password>
MKPL_EMAIL_SERVER = <mkpl_smtp_address>
MKPL_EMAIL_SERVER_PORT = <mkpl_smtp_port>
```

These environment variables can be stored in a .env file in the same directory as the docker-compose file.

The whole system can be started by using the command 

```shell
docker-compose up -d 
```

and stopped with the command 

```shell
docker-compose down
```

