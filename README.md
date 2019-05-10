
# Rancher-cli

Docker image based on alpine with :
- `rancher-cli` v2.2.0
- `kubectl` v1.13.2

# Usage

Launch the container
```bash
docker run --rm -it redfabriq/rancher-cli
```

Login to rancher

> You'll need an API key. See: https://rancher.com/docs/rancher/v2.x/en/user-settings/api-keys/#creating-an-api-key

```bash
rancher login --token <rancher_api_token> https://192.168.80.30/
```

Use kubectl (via rancher)
```bash
rancher kubectl get nodes
```
