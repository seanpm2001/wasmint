# wasmint
[![Build Status](https://travis-ci.org/Teemperor/wasmint.svg?branch=master)](https://travis-ci.org/Teemperor/wasmint)

A WebAssembly (**WASM**) **Int**erpreter licensed under the Apache 2.0 License.

## Binary format

As the binary format of WASM is still up to decision, this interpreter is currently using it's own 
binary format that tries to be as close as possible to the draft by the W3C group.
If you find any differences between the current binary format and the one from the draft, 
please create a issue on github.

For more information see the [documentation](docs/BinaryFormat.md).

## Building

wasmint requires a C++11 compiler (including STL) and CMake as build dependencies.

Make sure to pull all git submodules before the build:

```
git submodule init
git submodule update
```
### Linux/OS X/Unix/Posix

To build wasmint on those systems with cmake and make by running:

```
cmake . && make
```

You can also run the tests by running `ctest` in the build directory.

### Windows

On Windows you can use Visual Studio by generating a Visual Studio project through the CMake client or use 
ports of unix tools like the ones from MinGW.
