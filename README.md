<p align="center">
<img src="https://github.com/SuperiorOS/manifest/assets/29405483/4186221f-e198-43bf-a2d4-d1046a0db269" />
</p>

---

# Credits:

- [**SuperiorOS**](https://github.com/SuperiorOS)
- [**AOSP**](https://android.googlesource.com)
- [**LineageOS**](https://github.com/LineageOS)
- [**PixelExperience**](https://github.com/PixelExperience)
- [**ProtonAOSP**](https://github.com/ProtonAOSP)
- [**ArrowOS**](https://github.com/ArrowOS)
- [**Pixys OS**](https://github.com/PixysOS)
- [**Crdroid Android**](https://github.com/crdroidandroid)

To get started with the building process, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

# Requirements:

- Around 400G disk space.
- A computer with at least 16GB RAM running Linux (recommended) or MacOS.
- Build environment [setup](https://github.com/akhilnarang/scripts).

# Sync Source:-

```bash
repo init --no-repo-verify -u https://github.com/SuperiorExtended/manifest -b UDC -g default,-mips,-darwin,-notdefault
```
- If you don't care about commit history and want to save some space then:-
```bash
repo init --depth=1 --no-repo-verify -u https://github.com/SuperiorExtended/manifest -b UDC -g default,-mips,-darwin,-notdefault
```

```bash
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j$(nproc --all)
```

# Start the build:-

```bash
  . build/envsetup.sh
  lunch superior_<devicecodename>-<buildtype>
  mka bacon -j$(nproc --all)
```

---

# Some Links:-

- [**Telegram Public Chat**](https://t.me/superiorextendedsg)
- [**Telegram Channel**](https://t.me/superiorextendedos)
