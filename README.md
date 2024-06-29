# Sync

```
repo init -u ssh://git@github.com/hefatss/bengal_manifest -b bengal_515
```

```
repo sync -c -j$(nproc --all) --no-clone-bundle --no-tags --force-sync
```

# Build
```
 . build/envsetup.sh && lunch bengal-user && ./build.sh -j$(nproc --all) | tee log.xt
```
