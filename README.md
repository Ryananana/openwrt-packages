```yaml
sed -i '1i src-git custom https://github.com/kenzok8/openwrt-packages' feeds.conf.default
git pull
./scripts/feeds update -a
./scripts/feeds install -a
make menuconfig
```
