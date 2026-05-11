# linux_user

Role linux_user fully automate control of linux users

## Table of contents

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [linux_user_list](#linux_user_list)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.20`

## Default Variables

### linux_user_list

List linux users to be deployed to a target host.

**_Required:_** `true`<br />
**_Type:_** Dict<br />

#### Example usage

```YAML
linux_user_list:
  ansible:
    state: present
    shell: /bin/bash
    authorized_keys:
      - state: present
        key: public key value
    sudoers: config for sudoers file
```

## Dependencies

None.

## License

MIT

## Author

freedform
