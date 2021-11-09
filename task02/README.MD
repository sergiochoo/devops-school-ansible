ansible-vault encrypt secret.yml --vault-password-file vault-pass

ansible-playbook task02_create_users.yml --ask-vault-pass # or --vault-password-file vault-pass