# jn-legacy
Previous implementations of Jingle that are no longer updated.

## Rust instructions

To install the compiler on Linux: cargo build --release sudo cp ./target/release/jinglec /usr/local/bin/jinglec

To install stdlib: sudo mkdir /usr/local/lib/jinglec/ sudo cp std /usr/local/lib/jinglec/

Running the command `jinglec` will give instructions

## Python instructions

Installation:
  1. Clone project or download a release binary
  2. Install dependencies with `pip -r requirements.txt`
  
Compile to a native executable
  1. Run the following command `python3 -m compiler.compile <filename>`
  2. Run the generated executable

Generate LLVM bytecode
  1. Run the following command `python3 -m compiler.llvmgen <filename>`
  2. LLVM bytecode will be printed out

Execute in an LLVM JIT
  1. Run the following command `python3 -m compiler.run <filename>`
  2. Result will be printed

Execute a file on the virtual machine
  1. Run the following command `python3 -m compiler.vm <filename>`
  2. Result will be printed
