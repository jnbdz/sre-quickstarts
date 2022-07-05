# Linux | SRE | Quickstarts
## Setup
### Kali
You can quickly install useful packages for SRE in Kali: 
```bash
sudo apt install kali-tools-reverse-engineering
```
**Source:** https://www.kali.org/tools/kali-meta/#kali-tools-reverse-engineering
> **NOTE:** If you click on *Dependencies* you can see all the packages that will be installed.
## Comes with *Kali reverse engineering tools*
- [**apktool**](https://www.kali.org/tools/apktool/) [GitHub](https://ibotpeaches.github.io/Apktool/) - A tool for reverse engineering 3rd party, closed, binary Android apps. It can decode resources to nearly original form and rebuild them after making some modifications; it makes possible to debug smali code step by step. Also it makes working with an app easier because of project-like file structure and automation of some repetitive tasks like building apk.
- [**bytecode-viewer**](https://www.kali.org/tools/bytecode-viewer/) [GitHub](https://github.com/Konloch/bytecode-viewer) - This package contains Bytecode Viewer (BCV). It is an Advanced Lightweight Java Bytecode Viewer, GUI Java Decompiler, GUI Bytecode Editor, GUI Smali, GUI Baksmali, GUI APK Editor, GUI Dex Editor, GUI APK Decompiler, GUI DEX Decompiler, GUI Procyon Java Decompiler, GUI Krakatau, GUI CFR Java Decompiler, GUI FernFlower Java Decompiler, GUI DEX2Jar, GUI Jar2DEX, GUI Jar-Jar, Hex Viewer, Code Searcher, Debugger and more. There is also a plugin system that will allow you to interact with the loaded classfiles, for example you can write a String deobfuscator, a malicious code searcher, or something else you can think of. You can either use one of the pre-written plugins, or write your own. It supports groovy scripting. Once a plugin is activated, it will execute the plugin with a ClassNode ArrayList of every single class loaded in BCV, this allows the user to handle it completely using ASM. It’s currently being maintained and developed by Konloch.
- [**clang**](https://www.kali.org/tools/llvm-defaults/) []() - Clang project is a C, C++, Objective C and Objective C++ front-end for the LLVM compiler. Its goal is to offer a replacement to the GNU Compiler Collection (GCC). Clang implements all of the ISO C++ 1998, 11 and 14 standards and also provides most of the support of C++17.This is a dependency package providing the default clang compiler.
- [**dex2jar**](https://www.kali.org/tools/dex2jar/) [GitHub](https://github.com/pxb1988/dex2jar/tree/2.x) - dex-reader is designed to read the Dalvik Executable (.dex/.odex) format. It has a light weight API similar with ASM. An example here dex-translator is designed to do the convert job. It reads the dex instruction to dex-ir format, after some optimize, convert to ASM format. dex-ir used by dex-translator, is designed to represent the dex instruction dex-tools tools to work with .class files.
- [**edb-debugger**](https://www.kali.org/tools/edb-debugger/) [GitHub](https://github.com/eteran/edb-debugger) - edb is a graphical cross platform x86/x86-64 debugger. It was inspired by Ollydbg, but aims to function on x86 and x86-64 as well as multiple OS’s. Linux is the only officially supported platform at the moment, but FreeBSD, OpenBSD, OSX and Windows ports are underway with varying degrees of functionality.
    - [**edb-debugger-plugins**](https://www.kali.org/tools/edb-debugger/) - edb is a graphical cross platform x86/x86-64 debugger. It was inspired by Ollydbg, but aims to function on x86 and x86-64 as well as multiple OS’s. Linux is the only officially supported platform at the moment, but FreeBSD, OpenBSD, OSX and Windows ports are underway with varying degrees of functionality. This package provides the plugins that used by edb.
- [**jadx**](https://www.kali.org/tools/jadx/) [GitHub](https://github.com/skylot/jadx) - This package contains a Dex to Java decompiler. It contains a command line and GUI tools for produce Java source code from Android Dex and Apk files. Main features: - decompile Dalvik bytecode to java classes from APK, dex, aar and zip files - decode AndroidManifest.xml and other resources from resources.arsc - deobfuscator included. jadx-gui features: - view decompiled code with highlighted syntax - jump to declaration - find usage - full text search.
- [**javasnoop**](https://www.kali.org/tools/javasnoop/) [Google code](https://code.google.com/p/javasnoop/) - Normally, without access to the original source code, testing the security of a Java client is unpredictable at best and unrealistic at worst. With access the original source, you can run a simple Java program and attach a debugger to it remotely, stepping through code and changing variables where needed. Doing the same with an applet is a little bit more difficult. JavaSnoop attempts to solve this problem by allowing you attach to an existing process (like a debugger) and instantly begin tampering with method calls, run custom code, or just watch what’s happening on the system.
- [**jd-gui**](https://www.kali.org/tools/jd-gui/) [Homepage](http://jd.benow.ca/) - JD-GUI is a standalone graphical utility that displays Java source codes of “.class” files. You can browse the reconstructed source code with the JD-GUI for instant access to methods and fields.
- [**metasploit-framework**](https://www.kali.org/tools/metasploit-framework/) [Homepage](https://www.metasploit.com/) - The Metasploit Framework is an open source platform that supports vulnerability research, exploit development, and the creation of custom security tools.
- [**ollydbg**](https://www.kali.org/tools/ollydbg/) [Homepage](http://www.ollydbg.de/) - OllyDbg is a 32-bit assembler level analysing debugger for Microsoft Windows. Emphasis on binary code analysis makes it particularly useful in cases where source is unavailable.
- [**radare2**](https://www.kali.org/tools/radare2/) [Homepage](https://www.radare.org/) - The project aims to create a complete, portable, multi-architecture, unix-like toolchain for reverse engineering. It is composed by an hexadecimal editor (radare) with a wrapped IO layer supporting multiple backends for local/remote files, debugger (OS X, BSD, Linux, W32), stream analyzer, assembler/disassembler (rasm) for x86, ARM, PPC, m68k, Java, MSIL, SPARC, code analysis modules and scripting facilities. A bindiffer named radiff, base converter (rax), shellcode development helper (rasc), a binary information extractor supporting PE, mach0, ELF, class, etc. named rabin, and a block-based hash utility called rahash. This package provides the libraries from radare2.
- [**radare2-cutter**](https://www.kali.org/tools/radare2-cutter/) [Homepage](https://cutter.re/) - Cutter is a Qt based GUI for reverse engineering binaries, which makes use of the radare2 framework. Advanced users are expected to use the radare2 CLI tools instead, which are much more powerful.

## Command list
- `file` — determine file type
- `Tika` [Apache Tika](https://tika.apache.org/) (alternative to `file` command (more powerful)) toolkit detects and extracts metadata and text from over a thousand different file types (such as PPT, XLS, and PDF).
- `POI` [Apache POI](https://poi.apache.org/) Java API for Microsoft Documents (`Tika` uses Apache POI)
- `gst-typefind-1.0` [gst-typefind-1.0 - man pages section 1: User Commands | docs.oracle.com](https://docs.oracle.com/cd/E88353_01/html/E37839/gst-typefind-1-0-1.html) - Tool from GStreamer.
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
