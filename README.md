cloud3rsio.php
=========

Install php.

Installation
------------

```bash
$ ansible-galaxy install cloud3rsio.php
```

Requirements
------------

Nothing.

Role Variables
--------------

| Key | Default Value | Type |
| ------------- | ------------- | ------------- |
| `php_version` | `7.3.9` | Int |
| `php_dir` | `/usr/local/php` | String |
| `php_phpbuild_root` | `/usr/local/php-build` | String |
| `php_PHP_BUILD_EXTRA_MAKE_ARGUMENTS` | `-j2` | String |
| `php_configurations` | Reference to [defaults/main.yml](defaults/main.yml) | Array |
| `php_fpm_pool` | Reference to [defaults/main.yml](defaults/main.yml) | Hash |

Dependencies
------------

- `cloud3rsio.phpbuild`

Example Playbook
----------------

```yaml
- hosts: all
  roles:
    - role: cloud3rsio.php
      php_version: 7.3.9
```

License
-------

[MIT](LICENSE)

Author Information
------------------

- youyo
