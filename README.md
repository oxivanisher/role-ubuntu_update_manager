ubuntu_update_manager
=====================

This role configures the Ubuntu Update Manager. Currently it configures only which updates are shown.

As always: Use at your own risk!

Role Variables
--------------

| Name                          | Comment                                          | Default value |
|-------------------------------|--------------------------------------------------|---------------|
| ubuntu_update_manager_release | Which updates should the user be notified about. | `lts`         |

`ubuntu_update_manager_release` can be one of the following:
* normal
* lts
* never

Example Playbook
----------------
```yaml
- name: Configure Ubuntu Update Manager
  hosts: clients
  roles:
    - role: oxivanisher.linux_desktop.ubuntu_update_manager
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.linux_desktop](https://galaxy.ansible.com/ui/repo/published/oxivanisher/linux_desktop/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-linux_desktop).
