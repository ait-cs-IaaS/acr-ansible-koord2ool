# Ansible-Role: acr-ansible-koord2ool

AIT-CyberRange: Installs and runs limesurvey via docker-compose

## Requirements

- Debian or Ubuntu 
- Gitlab

## Role Variables

```yaml
--- ---
koord2ool_user: koord2ool
koord2ool_basepath: /opt/koord2ool

koord2ool_ssl_cert: /etc/ssl/server.crt
koord2ool_ssl_key: /etc/ssl/server.key

koord2ool_entry_point: 8080
koord2ool_lime_rpc_api: https://limesurvey.cyberrange.at/index.php/admin/remotecontrol
koord2ool_port: 8081
koord2ool_lime_admin_password: koord2ool_password
koord2ool_lime_admin_email: koord2ool@cyberrange.at
koord2ool_lime_public_url: https://limesurvey.cyberrange.at
koord2ool_lime_port: 8082

koord2ool_survey_lsa_files: []
```

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: koord2ool

```

## License

GPL-3.0

## Author

- Lenhard Reuter