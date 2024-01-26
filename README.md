### fix some bug when bulild for ghidra 11.0

# MCLFLoader

A Ghidra loader module for the MobiCore Loadable Format (MCLF) used by trustlet and driver binaries.

## Installation

Copy the ZIP file from the `dist/` to the `GHIDRA_INSTALL_DIR/Extensions/Ghidra` directory and install the module from the `File > Install extensions...` menu on the main screen.

## Compilation

Set the `GHIDRA_INSTALL_DIR` environment variable and run `gradle`.

cd DIR ; gradle -PGHIDRA_INSTALL_DIR=D:\Android\ghidra_11.0_PUBLIC

==========================
```
TA format: 
MDT: https://github.com/laginimaineb/unify_trustlet
MCLF: this loader
OP-TEE based: remove custom heaers, remain ELF file

file extensions: .tabin, .tlbin, .mbin, .ta, .sec
probably path: /mnt/vendor/persist/mcRegistry/, /vendor/app/mcRegistry/, /system/app/mcRegistry/

https://www.synacktiv.com/en/publications/kinibi-tee-trusted-application-exploitation
```
