<!-- Space: AnsibleRoleAuthorization -->
<!-- Parent: Project -->
<!-- Title: Project Examples -->

<!-- Label: Examples -->
<!-- Include: docs/disclaimer.md -->
<!-- Include: ac:toc -->

## Install

Install it with the following command:

```{.yaml}
ansible-galaxy install hadenlabs.authorization
```

### basic

To run this playbook with default settings, create a basic playbook like this:

```{.yaml}
- hosts: servers

  vars:
    user: ubuntu
    authorization_user: '{{ user }}'
    authorization_key_public: '~/.ssh/id_rsa.pub'
    authorization_key_private: '~/.ssh/id_rsa'

  roles:
    - hadenlabs.authorization
```
