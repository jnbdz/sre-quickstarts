# Linux | SRE | Quickstarts
## Setup
### Kali
You can quickly install useful packages for SRE in Kali: 
```bash
sudo apt install kali-tools-reverse-engineering
```
**Source:** https://www.kali.org/tools/kali-meta/#kali-tools-reverse-engineering
> **NOTE:** If you click on *Dependencies* you can see all the packages that will be installed.
## Command list
- `file` — determine file type
- `Tika` [Apache Tika](https://tika.apache.org/) (alternative to `file` command (more powerful)) toolkit detects and extracts metadata and text from over a thousand different file types (such as PPT, XLS, and PDF).
- `POI` [Apache POI](https://poi.apache.org/) Java API for Microsoft Documents (`Tika` uses Apache POI)
- `nm` - list symbols from object files
- `ldd` - print shared object dependencies
- `objdump` - display information from object files
- `otool` - object file displaying tool
- `c++filt` - demangle C++ and Java symbols
- `strings` - print the sequences of printable characters in files
- [`jadx`](https://github.com/skylot/jadx) - Dex to Java decompiler (in Kali: `sudo apt install jadx`)
- [`d2j-dex2jar`](https://github.com/pxb1988/dex2jar/tree/2.x) - Tools to work with android .dex and java .class files
- `ghidra` - ([Website](https://ghidra-sre.org/), [GitHub](https://github.com/NationalSecurityAgency/ghidra)) reverse engineering tool developed by the National Security Agency (NSA)

### Other Command list
- `readelf` - display information about ELF files
    - E.g.: `readelf -h /bin/bash`
- `size` - list section sizes and total size of binary files
