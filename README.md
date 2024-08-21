# Penfount bots configuration repository

## Inventory setup

Where ENV is an environment name (e.g. staging):

In ENV.yml inventory file, add the target host to a host group ENV.

## Secrets

Secrets should be stored in `group_vars/ENV.yml` and not committed.

## Run configuration

Ensure that your user on the target host has NOPASSWD `sudo` root privileges.

To run the playbook, where ENV is staging:

```shell
ansible-playbook -i staging.yml site.yml
```

