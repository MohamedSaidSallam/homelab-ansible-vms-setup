# homelab-ansible-vms-setup

## Usage

```sh
# WSL
# chmod 600 vault_pass
```

### Run everything

```sh
ansible-playbook vault_pass site.yaml
```

### Run specific playbook

example

```sh
ansible-playbook vault_pass setup-vms.yaml
```

```sh
ansible-playbook vault_pass setup-hv.yaml
```

## Configuration

[ansible.cfg](ansible.cfg)

## Vault

```sh
ansible-vault edit --vault-password-file vault_pass inventory/homelab/group_vars/all/vault/nexus.yaml
```
