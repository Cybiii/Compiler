# Programming Lang and Compiler

Making my own programming lanuage with a self-made compiler with NASM and GNU Linker in C++. Note: WSL might sometimes cause clock skews causing the CMake build fail. (project is a WIP)

## Handy commands:

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



