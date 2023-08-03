---
# Credits:

- [**AOSP**](https://android.googlesource.com)
- [**LineageOS**](https://github.com/LineageOS)
- [**ProtonAOSP**](https://github.com/ProtonAOSP)
- [**ArrowOS**](https://github.com/ArrowOS)
- [**Pixys OS**](https://github.com/PixysOS)
- [**Crdroid Android**](https://github.com/crdroidandroid)
- [**SuperiorOS**](https://github.com/SuperiorOS)

To get started with the building process, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

# Requirements:

- Around 400G disk space.
- A computer with at least 16GB RAM running Linux (recommended) or MacOS.
- Build environment [setup](https://github.com/akhilnarang/scripts).

# Sync Source:-

```bash
    repo init -u https://github.com/SuperiorExtended/manifest.git -b thirteen
```

```bash
    repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

# Start the build:-

```bash
  . build/envsetup.sh
  lunch superior_<devicecodename>-userdebug
  m bacon -j$(nproc --all)
```
