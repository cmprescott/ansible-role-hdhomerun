Ansible Role: HDHomeRun
=========

Installs HDHomeRun drivers.

Requirements
------------

```shell
# Ansible version 1.4.4+
ansible --version

# OS
case $OSTYPE in
  # Linux needs apt
  "linux"*)
      apt --version;;
esac
```


Role Variables
--------------

```yaml
hdhomerun_dvb_apt_repo: "ppa:r3gis-r3gis/dvbhdhomerun"
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: clients.media
  roles:
    - name: "Ensure HDHomeRun's drivers"
      role: cmprescott.HDHomeRun
      sudo: Yes
```

License
-------

BSD

Author Information
------------------

Prescott Chris
