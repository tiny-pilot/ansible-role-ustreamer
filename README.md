# Ansible Role: µStreamer

[![CircleCI](https://circleci.com/gh/mtlynch/ansible-role-ustreamer.svg?style=svg)](https://circleci.com/gh/mtlynch/ansible-role-ustreamer) [![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-ustreamer-blue.svg?style=flat-square)](https://galaxy.ansible.com/mtlynch/ustreamer) [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](LICENSE)

Ansible role for [µStreamer](https://github.com/pikvm/ustreamer).

## Role Variables

Available variables are listed below, along with default values (see [defaults/main.yml](defaults/main.yml)):

```yaml
ustreamer_group: ustreamer
ustreamer_user: ustreamer
ustreamer_dir: /opt/ustreamer
ustreamer_repo: https://github.com/pikvm/ustreamer.git
ustreamer_interface: '0.0.0.0'
ustreamer_port: 8001
ustreamer_video_path: /dev/video0
```

## Dependencies

None

## Example Playbook

#### `example.yml`

```yaml
- hosts: all
  roles:
    - role: mtlynch.ustreamer
```

### Running Example Playbook

```bash
ansible-galaxy install mtlynch.ustreamer
ansible-playbook example.yml
```

## License

MIT

## Author Information

This role was created in 2020 by [Michael Lynch](http://mtlynch.io).