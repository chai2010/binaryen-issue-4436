# binaryen-issue-4436
https://github.com/WebAssembly/binaryen/issues/4436

https://github.com/WebAssembly/binaryen/releases/tag/version_104

macOS 12.0.1 (21A559)

```
$ md5sum libbinaryen.dylib 
8a38a255d8ceb1b53986bd0f838f07d9  libbinaryen.dylib
$ md5sum main.c 
$ clang --version
Apple clang version 13.0.0 (clang-1300.0.29.3)
Target: x86_64-apple-darwin21.1.0
Thread model: posix
InstalledDir: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin
$ clang main.c libbinaryen.dylib 
$ md5sum a.out 
ea1f12aa44c01720b272b8cfbf2268f3  a.out
$ ./a.out 
dyld[25913]: missing symbol called
Abort trap: 6
```
