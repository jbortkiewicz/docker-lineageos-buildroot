# docker-lineageos-buildroot

## Troubleshooting
### grsec and java
On kernels with **grsecurity** patch applied like **_standard_ Apline Linux**, the compilation process will fail on starting Java process with an error similar to the following:
```
OpenJDK 64-Bit Server VM warning: INFO: os::commit_memory(0x0000029c7d000000, 2555904, 1) failed; error='Operation not permitted' (errno=1)
```
To resolve this issue use normal Linux kernel e.g. **_vanilla_ Apline Linux** or change PaX flags using `paxctl` tool (I haven`t done this)
