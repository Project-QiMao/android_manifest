# Project-QiMao

## Getting Started

To get started with the AcmeUI sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

### 1. Initialize your local repository
```bash
repo init -u https://github.com/Project-QiMao/android_manifest.git -b seagull
```
or
```bash
repo init -u https://github.com/Project-QiMao/android_manifest.git -b seagull --depth=1
```

### 2. Sync up
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### 3. Clone your device sources repositories

### 4. Initialize the ROM environment with the envsetup.sh script
```bash
source build/envsetup.sh
```

### 5. Lunch your device
```bash
lunch qimao_<$device_name>-<$buildtype>
```

### 6. Start compilation
```bash
mka qimao
```