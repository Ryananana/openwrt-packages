[![Custom Repository Sync](https://github.com/Ryananana/openwrt-packages/actions/workflows/sync.yaml/badge.svg)](https://github.com/Ryananana/openwrt-packages/actions/workflows/sync.yaml)

```yaml
sed -i '1i src-git custom https://github.com/Ryananana/openwrt-packages' feeds.conf.default
git pull
./scripts/feeds update -a
./scripts/feeds install -a
make menuconfig
```
