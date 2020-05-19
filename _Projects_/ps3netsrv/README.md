# ps3netsrv

## Requirements

* A C/C++ compiler

* [Meson](https://mesonbuild.com/Getting-meson.html)

* [mbed TLS](https://tls.mbed.org/)
  * Is being searched for in system library directory (e.g. `/usr/lib`) and custom directories specified in `LIBRARY_PATH`.
  If using a custom directory, put the path to the headers in `C_INCLUDE_PATH`.

`Meson` and `mbed TLS` are available as packages for most posix environments.

## Building

First configure a build directory:

```bash
$ meson buildrelease --buildtype=release
```

Then build using ninja:

```bash
$ ninja -C buildrelease
```

For further information see [Running Meson](https://mesonbuild.com/Running-Meson.html).

## Notes
Use _make.bat in Windows or Make.sh in linux to build ps3netsrv using POLARSSL library instead of mbed TLS and without Meson


## Docker Container
Docker Engine enables applications built in containers packages to run anywhere consistently on any infrastructure.

Docker container packages for ps3netsrv are available at:
https://hub.docker.com/search?q=ps3netsrv