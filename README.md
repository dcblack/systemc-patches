# Experimental

This directory contains a single file comprising some patches I am working on against the SystemC PoC source taken from https://github.com/accellera-official/systemc. At some point, I may propose some of these to the committee. In the meantime, these are experimental. Apply at your own risk.

PATCHING SYSTEMC
----------------

These SystemC patches should not break anything and are quite limited. At present, the patches have only been applied to the Accellera Official repository and compiled using the "experimental" cmake approach, which I find to be simpler and more stable. 

Obtain a copy of my latest patches from <https://github.com/dcblack/systemc-patches.git>

Here are the steps:

1. Build SystemC

2. Go to the source directory and do the following:

```bash
git am --empty=drop "PATH_TO_HERE/systemc.patches"
cmake -B build
cmake --build build
cmake --install build
```

Good luck!
