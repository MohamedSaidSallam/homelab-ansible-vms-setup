# homelab-ansible-vms-setup

## Usage

```sh
# WSL
# chmod 600 vault_pass
```

### Run everything

```sh
ansible-playbook -i inventory/homelab/ --vault-password-file vault_pass site.yaml
```

### Run specific playbook

```sh
ansible-playbook -i inventory/homelab/ --vault-password-file vault_pass setup-vms.yaml
```

```sh
ansible-playbook -i inventory/homelab/ --vault-password-file vault_pass setup-hv.yaml
```

## Vault

```sh
ansible-vault edit --vault-password-file vault_pass inventory/homelab/group_vars/all/vault/nexus.yaml
```
