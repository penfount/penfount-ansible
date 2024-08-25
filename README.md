# Penfount bots configuration repository

## Inventory setup

Where ENV is an environment name (e.g. staging):

In ENV.yml inventory file, add the target host to a host group ENV,
and add secrets as group varibles. See `inventory-example.yml`.

## Run configuration

Ensure that your user on the target host has NOPASSWD `sudo` root privileges.

To run the playbook, where ENV is staging:

```shell
ansible-playbook -i staging.yml site.yml
```

