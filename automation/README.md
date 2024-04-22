# Install Infra
`install-infra` will perform the full infrastructure installation via Ansible automation. 

This includes:
* Installing ACM to OCP hub cluster
* Installing ACS via ACM subscription to hub and managed clusters

Example:
```
ansible-playbook install-infra.yaml --vault-password-file=~/.passfile
```

# Install ACM
`install-acm` installs ACM to the hub cluster using an Operator Subscription.

Example:
```
ansible-playbook install-acm.yaml --vault-password-file=~/.passfile
```

# Install ACS via ACM Subscription
`install-acs-via-acm-policy` installs ACS to the hub and managed clusters using ACM policies, created using a Subscription.

Example:
```
ansible-playbook install-acs-via-acm-policy.yaml --vault-password-file=~/.passfile
```
