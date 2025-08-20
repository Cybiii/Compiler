# Compiler-test

Trying to make my own compiler with NASM and GNU Linker in C++. Note: WSL might sometimes cause clock skews causing the build fail.

Handy commands:

Assembler (object file):

```
nasm -felf64 test.asm
```

Linker (executable):

```
ld test.o -o test
nasm -felf64 test.asm && ld test.o -o test && ./test
```

Compile main.cpp into hydro

```
cd hydrogen
cmake -S . -B build/ && cmake --build build/
./build/hydro ./test.hy
```
