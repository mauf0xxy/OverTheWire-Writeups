# Level 12 → Level 13
> Convert the hexdump back to raw binary
> 

---

```bash
xxd -r data.txt > data.bin
file data.bin
```

- if file says gzip compressed data

```bash
mv data.bin data.gz
gunzip data.gz
```

- if file says bzip2 compressed data

```bash
mv data.bin data.bz2
bunzip2 data.bz2
```

- if file says POSIX tar archive

```bash
mv data.bin data.tar
tar -xf data.tar
```
---

**`xxd -r`** — **Reverse Hex Dump** converts a plaintext hexadecimal dump back into its original binary file format

**`mv`** — **Move** files from one directory to another, or **renames** them

**`file`** — **Identify File Type**

**`gunzip`** — **Decompress Gzip** (usually ending in **`.gz`**)

**`bunzip2`** — **Decompress Bzip2** (usually ending in **`.bz2`**)

**`tar -xf`** — **Extract Tarball,** The **`-x`** flag tells it to extract, and **`-f`** specifies the file