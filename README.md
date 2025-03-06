# NOKIA-DTECH-BUILD
Nokia DTech buid

## Installing Ansible Collection
Installing ansible collection

```sh
# ansible-galaxy collection install git+https://github.com/kwozyman/vpac.git,master
# Since PR is not merged and changes are sitting in my fork lets install collection from my fork
ansible-galaxy collection install git+https://github.com/rprakashg-rh/vpac.git,master
```

## Steps to create Ansible Vault


Run command below

```sh
ansible-vault create vars/secrets.yml
```

Enter a password for Vault and hit enter which will bring up an editor. Add the yaml snippet below replacing the redacted sections

```yaml
admin_user: '<<redacted>>'
admin_password: '<<redacted>>'
admin_ssh_key: '<<redacted>>'
rootpw: '<<redacted>>'
```

Set the Vault secret into an environment variable as shown below

```sh
export VAULT_SECRET="<<redacted>>"
```



