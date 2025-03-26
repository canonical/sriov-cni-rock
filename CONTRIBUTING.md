# Contributing

## Build and deploy

```bash
sudo snap install rockcraft --classic --edge
rockcraft pack -v
sudo rockcraft.skopeo --insecure-policy copy oci-archive:sriov-cni_2.9.0_amd64.rock docker-daemon:sriov-cni:2.9.0
docker run -d sriov-cni:2.9.0
```
