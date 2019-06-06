LineageOS
===========

Getting started
---------------

```
1. mkdir -p LOS && cd LOS

2. Initialize your local repository using the LineageOS trees with a command
  repo init -u git://github.com/LineageOS/android.git -b cm-13.0
  
3. Clone this repo:
  git clone https://github.com/CustomROMs/android_local_manifests_u8500 .repo/local_manifests -b cm-13.0

4. Sync LineageOS trees:
  repo sync --no-tags --no-clone-bundle --force-sync -c -j8

5. Apply patches:
  . build/envsetup.sh
  cd device/samsung/codina/patches
  . patcher.sh apply
  cd ../../../../

6. To build:
  . build/envsetup.sh
  lunch lineage_codina-userdebug
  make -j8 bacon
```
