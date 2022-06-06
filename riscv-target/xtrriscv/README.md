# XtrRiscv
## Requirements
- [Modelsim/Questa](https://www.intel.com/content/www/us/en/collections/products/fpga/software/downloads.html?edition=lite&s=Newest)
- [RISC-V compiler](https://github.com/sifive/freedom-tools/releases)
- make
- hexdump
```bash
$ apt-get install make bsdmainutils
```

## Setting up
Before running the tests, you'll need to set the following variables.
```bash
$ export TARGET_SIM="vsim -work XTRRISCV_REPO/rtl/proj/modelsim/work"
$ export RISCV_PREFIX=PATH_TO_BIN_RISCV_COMPILER
```

Make sure that the modelsim project is generated and compiled. 
Check **[Compiling the testbench](https://github.com/Pedroo64/XtrRiscv/tree/master/rtl/proj/modelsim/README.md#compiling-the-testbench)** section how to create and compile the Modelsim project.

## Running tests

To run the tests, go to the root of this repository and enter the following command : 
```bash
$ make RISCV_TARGET=xtrriscv RISCV_DEVICE=I
```
