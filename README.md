FreeBSD .NET (dotNET) Crossbuilt under Linux using GHA

Build logic taken from https://github.com/filipnavara/dotnet-riscv

Adapted for FreeBSD both AMD64 (x64) and ARM64. Currently only NET11.

Works for NET10 after changing tag logic and container.

Does no additional patching. FreeBSD Ports version has some extra [patches](https://github.com/freebsd/freebsd-ports/tree/main/lang/dotnet/files)

This is all done automagically. Checks for new tags daily. Failed builds/tags are rerun every day. 

If you want the the SDK from FreeBSD Ports use `pkg install dotnet`. This is easiest way of using the SDK.

FYI to people wanting to private repo fork this: GHA eat minutes like popcorn (90min per arch per tag)

Otherwise, enjoy!
