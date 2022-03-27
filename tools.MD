# Disassemblers

## IDA Pro
Advantages:
    - Names to functions, variables, data structures
    - Change data representation(as numbers, strings in various encodings,
    data structures)
    - Build diagrams and code flow graphs to simplify the understanding of
    disassembled code
    - Use type information about function arguments and structure definitions
    from C++ so that arguments and variables are automatically named
    - Recognize and name standard library functions in assembler code
### Plugins
Hex-Rays Decompiler
Lighthouse - marks pieces of code depending on how many times they were executed
ClassInformer
    - For binaries built in Visual Studio
    - Searches for RTTI information stored in the data section
    - RTTI allows the plugin to find the class names and virtual methods of
    C++ classes
Bindiff:
    - Compare binaries as assembler code instead of stream of bytes
    - Changes can also be represented as code flow graphs
IDA-function Tagger:
    - Analyzes imported functions and groups them by tags:
    Cryptography-related, registry-related, network-related, etc.
ida-x86emu:
    - Emulate the result of executing any piece of code without the risk of
    modifying something in the system. Just need to specify the start values
    of the CPU registers.
## Binary Ninja
## Ghidra
## Cutter
## Hopper

# Decompilers
## dnSpy
.NET decompiler
## .NET reflector
## JustDecompile
## IDA
## Ghidra
## Bytecode Viewer
Java Decompiler(also for android apps)
## Java decompiler
## REFox
## VB Decompiler
## IDR
Interactive Delphi Reconstructor

# Application Packages
MSI
DELPHI
Borland
PKG
DMG


# Emulators/Boxes
Sandboxie
Qemu

# Debuggers
## x32dbg, x64dbg
Plugins, visual themes
## OllyDbg
## DILE
DotNet IL Editor

# Editing Binaries
## CFF explorer
PE and HEX editors
Resource editor
Import editor
Signature scanner
Address converter
Disassembler
Dependency analyzer
More??

## Relocation Section Editor
Editing the relocation table in PE files.
Modify the relocation table in case of patching relocatable pieces of code.
Often used to remove the relocation table altogether when restoring a
protected file.
A protected file actually contains the relocation table for the unpacker code
only. The relocation table for the real code is usually hidden within the
unpacker data.
In case a dump is being recovered, there are two ways to restore the missing
relocation table for the real code:
1. Force the application to be loaded at 2 different base addresses, then
compare the dumps to see which parts of the code are being patched and
make a new relocation table.
2. Remove the relocation table completely and specify in the PE file header
that the file is not relocatable.

## Resource Hacker
Find things like raw binary data, dialogs, bitmaps, strings, icons.
It allows you to modify it or replace it with your own versions.

## Resource Hacker FX
## Resource Tuner
## PE-bear
## DityJoe
Advanced editor for compiler Java files.

# For Unpacking/Anti-RE
## PEiD
By analyzing entropy, PEiD can detect whether and application is packed.
## KANAL
- Krypto Analyzer for PEiD
## Detect It Easy
## ProtectionID
## de4dot
## PE Explorer

# Viewers
## PeStudio
## PE-bear

# Yara
Yara Gui

# Monitoring
## API Monitor
## ProcessExplorer
## ProcessMonitor

# Hex Editors
## WinHex
## Hiew
- Built-in disassembler for x86, x86-64, ARM
- Viewing and editing logical and physical drives
- Searching for assembler commands by template
- Keyboard macros
- Built-in 64-bit calculator
- Tools to create custom plugins
## Hex workshop
## HxD

# Network proxies
## Fiddler
Monitor, analyze traffic
Also supports plugins(wbxml view)
Built-in hex editor and can generate requests based on a selected request or
create a custom request.
Request to code Plugin
## Wireshark

# Memory dumpers
## Scylla
Dumping a running application process and restoring the PE import table
You can get a totally restored PE file that can be run by the operating system
