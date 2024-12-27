# Sync

```
repo init -u https://github.com/ShelbyHell/bengal_manifest -b bengal_515 -g default,-mips,-darwin,-notdefault
```

```
repo sync -c -j$(nproc --all) --current-branch --no-clone-bundle --no-tags --force-sync
```

# Build
```
 . build/envsetup.sh && lunch bengal_515-user && ./build.sh -j$(nproc --all) | tee log.txt
```