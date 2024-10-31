Ansible Role: Launch Nutanix Blueprint
=========
An Ansible Role that launch Blueprint on Nutanix Cluster.

Requirements
------------
none.

Role Variables
--------------
Available variables are listed below, along with default values (see defaults/main.yml):

```yaml
# Instance Configuration
pc_ip: <PC-IP>
vm_name: <VM-NAME>
substrate_list_uuid: <SUBSTRATE-LIST-UUID>

# Application Configuration
app_name: <APP-NAME>
app_description: <APP-DESC>

# Blueprint & Profile
bp_id: <BP-UUID>
app_profile_reference_name: <TSHIRT-SIZE>
app_profile_reference_uuid: <APP-UUID>
card_id: <CARD-ID>
card_uuid_variable: <card_uuid_varible>

# Credentials
username: <VM-USERNAME>
password: <VM-PASSWORD>
basic_auth: <PC-BASIC-AUTH>
username_uuid_variable: <uuid_variable>
password_uuid_variable: <uuid_variable>
```

Dependencies
------------
none.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
- hosts: servers
  roles:
      - { role: arguxx.launch_simple_blueprint }
```

License
-------
BSD

Author Information
------------------
This role was created in 2024 by Argian Raditya.