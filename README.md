# Coral Gasket Driver

The Coral Gasket Driver allows usage of the [Coral EdgeTPU](https://coral.ai/) on Linux systems. The driver contains two modules:

* Gasket: Gasket (Google ASIC Software, Kernel Extensions, and Tools) is a top level driver for lightweight communication with Google ASICs.
* Apex: Apex refers to the [EdgeTPU v1](https://coral.ai/technology)

This repo contains both the source for direct integration into a kernel tree as well as the necessary files to generate a Debian DKMS package.

## Building Debian DKMS package

From the top level directory, execute:

```
debuild -us -uc -tc -b
```
