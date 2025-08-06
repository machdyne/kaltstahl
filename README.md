# Kaltstahl Storage Device

Kaltstahl is a higher capacity version of [Blaustahl](https://github.com/machdyne/blaustahl).

Please see the [Blaustahl](https://github.com/machdyne/blaustahl) repo for instructions and firmware source code.

To build the firmware from the source code, you will need to modify blaustahl.h and change the FRAM\_SIZE value to 262144 and then use the following commands:

```
$ mkdir build
$ cd build
$ cmake -DPICO_DEFAULT_BOOT_STAGE2_FILE=/your-pico-sdk-directory/pico-sdk/src/rp2040/boot_stage2/boot2_generic_03h.S ..
$ make
```

## License

The contents of this repo are released under the [Lone Dynamics Open License](LICENSE.md).
