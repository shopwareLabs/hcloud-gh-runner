# Hetzner Cloud GitHub Runner

GitHub right now does not offer arm64 runners. So we set up our own at Hetzner Cloud.


## Create server

```
op run --env-file .env -- ansible-playbook create.yml
```

## Provision them

```
op run --env-file .env -- ansible-playbook provision.yml
```