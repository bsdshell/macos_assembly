### MacOS Assembly Hello World, Big Sur 11.5.2

## Install yasm on MacOS if you need.
```
  brew install yasm 
  yasm -f macho64 hello.asm
  ld -L /Library/Developer/CommandLineTools/SDKs/MacOSX.sdk/usr/lib -lSystem -o hello hello.o

  // ERROR: ld -lSystem -o hello hello.o
  // ld can not locate the lib path 
```
[[https://rderik.com/blog/let-s-write-some-assembly-code-in-macos-for-intel-x86-64/]ref]


