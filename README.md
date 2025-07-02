# xoa-installer-role

Ansible wrapper to manage XenInstallerUpdater script.

## Basic play example

```yaml
...
- name: XOA
  hosts: xoa
  become: true
  tasks:
    - name: XOA-update-script
      ansible.builtin.include_role:
        name: xoa-installer-role
      vars:
        xo_domain: "xoa.example.io"
        xo_cert_common_name: "xoa"
        xo_web_banner_tweak: true
...
```
