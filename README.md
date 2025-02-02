# Kaltstahl Storage Device

Kaltstahl is a higher capacity version of [Blaustahl](https://github.com/machdyne/blaustahl).

Please see the [Blaustahl](https://github.com/machdyne/blaustahl) repo for instructions and firmware source code.

To build the source code, you will need to modify blaustahl.h to uncomment FRAM\_BIG, set FRAM\_PAGES to 128 and then use the following commands:

```
$ mkdir build
$ cd build
$ cmake -DPICO_DEFAULT_BOOT_STAGE2_FILE=/your-pico-sdk-directory/pico-sdk/src/rp2_common/boot_stage2/boot2_generic_03h.S ..
$ make
```

## License

The contents of this repo are released under the [Lone Dynamics Open License](LICENSE.md).
