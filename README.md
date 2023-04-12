# Sync

```
repo init -u ssh://git@github.com/chrisl7/bengal_manifest -b LA.UM.9.15.2.r1
```

```
repo sync -c -j$(nproc --all) --no-clone-bundle --no-tags --force-sync
```

# Build
```
 . build/envsetup.sh && lunch bengal-user && ./build.sh -j$(nproc --all) | tee log.xt
```
