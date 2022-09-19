# Fedora 36 GCC 12 pico-sdk linker warning

Demonstrates the linker warning present when compling pico-sdk with GCC 12
shipped with Fedora 36.

```
[1/5] Performing build step for 'ELF2UF2Build'
ninja: no work to do.
[5/5] Linking CXX executable hello_world.elf
/usr/lib/gcc/arm-none-eabi/12.2.0/../../../../arm-none-eabi/bin/ld: warning: hello_world.elf has a LOAD segment with RWX permissions
/usr/lib/gcc/arm-none-eabi/12.2.0/../../../../arm-none-eabi/bin/ld: warning: hello_world.elf has a LOAD segment with RWX permissions

```


## Quickstart

```
mc fedora:36 cmake -G Ninja -Bbuild -S.
mc fedora:36 ninja -C build
```

