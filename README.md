# asm

assembly

---

### Code

```asm
global _main

section .text
_main:
    NOP
    NOP
    NOP
    NOP
    NOP
    NOP
    NOP
    MOV EAX, 41424344h ; ABCD
    MOV BX, 4141h
    MOV CH, 41h
    MOV DL, 41h
```

### Object file

```bash
nasm -f win32 code.asm
```

### Disassembly .obj

```bash
objdump -d -M intel code.obj
```

> INTEL Syntax

```bash
objdump -d code.obj
```

> AT&T Syntax

---

## Resources

- [Nasm](https://www.nasm.us/)
- [Objdump](https://www.mingw-w64.org/source/)
- [Golinker](http://www.godevtool.com)
