# Pixel Experience #

### Sync ###

```bash

# Initialize local repository
repo init --depth=1 -u https://github.com/PixelExperience-MiA2-Mi6X/manifest -b twelve

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --optimized-fetch
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

### Submitting Patches ###

Patches are always welcome! Please submit your patches to our Gerrit.

[Gerrit push guide](https://wiki.pixelexperience.org/help/submit-patch/)
