# Ansible Role: MySQL Container
This role creates MySQL container on target host.  

# Requirements
Target host must be running Docker enginer and have Docker PIP module installed.  

# Role Variables
Please refer to [defaults/main.yml](./defaults/main.yml) for variables' description and example values.  

# Dependencies
None.  

# Example playbook
```
- hosts:
    - mysql_server
  roles:
    - role: almaops.ct_mysql
      ct_mysql_env_mysql_root_password: "my_root_pw"
      ct_mysql_env_extra:
        MYSQL_DATABASE: sample_db
        MYSQL_USER: sample_user
        MYSQL_PASSWORD: sample_password
```

# License
[MIT](./LICENSE)

# Contributors
[Valentin Gostev](https://github.com/ussrlongbow).  
