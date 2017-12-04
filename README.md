Ansible role for Nginx installation on EL/AWS Linux
---

# Role variables

```yml
---

nginx_user: nginx                                       # default user
nginx_conf_file: /etc/nginx.conf                        # path to your conf file
nginx_pidfile: /var/run/nginx.pid                       # pidfile location
nginx_programs_dir: /etc/nginx/conf.d/                  # child programs location
nginx_sites_enabled: /etc/nginx/site-enabled/
nginx_logfile: /var/log/nginx/access.log
nginx_errlog: /var/log/nginx/error.log
```

# Dependencies

* Mallear.yum

# Example

```yml
- hosts: localhost
  remote_user: root
  roles:
    - Mallear.nginx-el
```