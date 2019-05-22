- To create user, please edit variable user_name in folder group_vars, and copy autherized_keys (public key) to roles/Copy_Key/
change file main.yml as:

```
roles:
    - Create_User
    - Copy_Key
    #- Delete_User
```

- To delete user, please edit variable user_name in folder group_vars, change file main.yml as:

```
roles:
    #- Create_User
    #- Copy_Key
    - Delete_User
```

run:
`sudo ansible-playbook -i hosts main.yml`
