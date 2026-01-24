# WineHQ | SRE | Quickstarts

## Setup
```bash
apt install gdb-mingw-w64 gdb-mingw-w64-target
```

Run program: 

```bash
wine Z:/usr/share/win64/gdbserver.exe localhost:12345 myprogram.exe
```

From another terminal screen: 

```bash
x86_64-w64-mingw32-gdb myprogram.exe
    (gdb) set solib-search-path ...directories with the DLLs used by the program...
    (gdb) target extended-remote localhost:12345
```

> `gdbserver` works better than `winedbg --gdb`.

## Resources
### Websites
- [How to properly debug a cross-compiled Windows code on linux? - StackOverflow](https://stackoverflow.com/questions/39938253/how-to-properly-debug-a-cross-compiled-windows-code-on-linux/68268087#68268087)
### Videos
- [ RARE 002: Debugging #Wine Apps with #Ghidra - YouTube](https://www.youtube.com/watch?v=Id-05jVepW0)
