<p>
  <d><strong>ollvm-23</strong></d>
  <br/>
  <sup>obfuscator llvm 23</sup>
  <br/>
</p>

<p>ollvm (obfuscator llvm) plugin ported to llvm 23.1.1. add bogus control flow, flattening, splitting, substitution to obfuscate your C/C++ code.</p>

## usage:

**use with clang:**
```
clang -fpass-plugin=libObfuscation.so -mllvm -fla -mllvm -bcf -mllvm -sub -mllvm -split file.c -o output-file
```

**compile:**

*llvm installed via brew:*

```
cd ollvm && mkdir build && cd build && cmake ../obfuscation && make
```

*llvm anywhere else:*
```
cd ollvm && mkdir build && cd build && cmake -DLLVM_DIR=<llvm location> ../obfuscation && make
```

---

<sup>this repo was created as part of the  `obsidian protector - universal pe packer` project found [here](https://github.com/vertigo6622/obsidian-protector)</sup>
