
# Ansible Role: kubectl

[![CI](https://github.com/sgaunet/ansible-role-kubectl/workflows/CI/badge.svg)](https://github.com/sgaunet/ansible-role-kubectl/actions?query=workflow%3ACI)

An Ansible Role that installs kubectl on Linux.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    kubectl_version: "1.27.7"
    kubectl_bin_path: "/usr/bin"
    kubectl_tmp_directory: "{{ lookup('env', 'TMPDIR') | default('/tmp', true) }}"
    kubectl_os: "linux"
    kubectl_arch: "amd64"

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - sgaunet.kubectl
```

## License

MIT
