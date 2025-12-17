## Changelog v1.4.5

References | Description | Author(s)
--- | --- | ---
#1254 | Bump bundled fmt to 12.0.0 | @deckstose
#1242 | Enable vim movement in help menu | @botantony
#948 | Remove reduntant symbols in tree view | @Denizantip
#1249 | Use /sys/dev/block/MAJOR:MINOR instead of /sys/block/NAME for disk I/O | @CountBleck
#1227 | feat: display CPU power draw & fix GPU+load avg overwriting core info | @Tom94 and @YuriiShkrobut
4f5abbb | Fix locale issues | @aristocratos
#1165 | Add encode and decode meters on Nvidia GPUs | @sam-kirby
#1197 | linux: Battery Time-to-full | @RadsammyT
#1203 | Convert ascii escape codes in mountpoint names before reading statvfs | @deckstose
#1198 | Fix presets erroring with gpu* usage | @entropylost
#1191 | Fix --tty/--no-tty flag having no effect | @deckstose

Big thanks to @deckstose for helping out with project maintenance, PR reviews and merging!

**For additional binaries see the [Continuous Builds](https://github.com/aristocratos/btop/actions).**

**Linux binaries for each architecture are statically linked with musl and works on kernel 2.6.39 and newer.**

**No MacOs or BSD binaries provided for the moment.**

**Notice! None of the binaries have GPU support, compile yourself or wait for distribution packages for GPU monitoring support!**

**Notice! Use x86_64 for 64-bit x86 systems, i486 and i686 are 32-bit!**
