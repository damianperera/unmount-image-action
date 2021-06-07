# Unmount Image Action
An action that unmounts an image's `boot` and `root` partitions inside a Ubuntu runner, ideally created by the [damianperera/mount-image-action@v1](https://github.com/damianperera/mount-image-action) action.

# Example
```
- name: Unmount Image
  uses: damianperera/unmount-image-action@v1
  with:
    imagePath: /home/github-runner/rpi4.img
    bootDeviceMapper: /dev/mapper/loop5p0
    rootDeviceMapper: /dev/mapper/loop5p1
```
For a usage example refer [this workflow file](https://github.com/damianperera/openwrt-rpi/blob/main/.github/workflows/build.yml).
