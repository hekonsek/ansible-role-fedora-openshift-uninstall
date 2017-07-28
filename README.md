# Ansible role: Login operation for OpenShift Origin on Fedora

Ensures that: 
- OpenShift service is stopped and removed
- OpenShift volumes are removed 
- `oc` and `oadm` clients are removed

## Compatibility

This playbook has been tested against Fedora 25.

## Installation 

    ansible-galaxy install hekonsek.fedora-openshift-uninstall,0.0

## Example playbook

    - hosts: localhost
      remote_user: root
      roles:
        - { role: hekonsek.fedora-openshift-uninstall,0.0 }

## License

Apache 2.0
