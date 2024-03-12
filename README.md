# homelab-ansible-vms-setup

## Usage

```sh
# WSL
# chmod 600 example_vault_pass

ansible-playbook -i inventory/homelab/ --vault-password-file example_vault_pass  playbooksssss.yaml
```

## Vault

```sh
ansible-vault edit --vault-password-file example_vault_pass inventory/example/group_vars/all/vault/nexus.yaml
```
