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