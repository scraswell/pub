# HomeLab Cloud Init Bootstrapping
## Building
To build the user-data and meta-data files, which will be placed in the ./dist
folder, execute:
```sh
pnpm build
```

## From Arch Linux Install CD
Add the following kernel parameters when booting the install CD:
```bash
ds=nocloud-net;s=https://scraswell.github.io/pub/cloud-init/ my_cloud_init_config={"user":"{username}","hostname":"{somehostname}"}
```