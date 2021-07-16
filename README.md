# Nortical UI #

![Nortical logo](https://chiakijudge.site/img/Banner.png)

### Sync ###

```bash
# Initialize local repository
repo init -u https://chiakijudge.site/Nortical-UI/platform_manifest -b 11-R

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash
# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```
