
<!--![Nortical logo](https://github.com/Nortical-UI/platform_manifest/blob/12-S/nortical.png)-->

# <img src="https://github.com/Nortical-UI/platform_manifest/blob/12-S/nortical.png" width="210">  Nortical UI Project #

### Introduction ###

What is *Nortical UI* ?

Nortical UI is a third-party ROM project supported by community developers.

Contributions are welcomed through pull requests.

([Rubik](https://hubertfischer.com/work/type-rubik) font is used in 2021 version of logo. )

### To Sync ###

```bash
# Initialize local repository
repo init -u https://github.com/Nortical-UI/platform_manifest -b 12-S

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --fail-fast
```

### To Build ###

```bash
# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch nortical_$device-userdebug

# Build!
$ make konata -j$(nproc --all)
