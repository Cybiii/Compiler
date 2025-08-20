# Compiler-test

Trying to make my own compiler with NASM nad GNU Linker goes wrong

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
