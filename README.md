# Sync

```
repo init -u https://github.com/edward0181/holi_manifest.git -b LA.UM.9.14.1.r1
```

```
repo sync -c -j$(nproc --all) --no-clone-bundle --no-tags --force-sync
```

# Build
```
 . build/envsetup.sh && lunch holi-user && ./build.sh -j$(nproc --all) | tee log.xt
```
