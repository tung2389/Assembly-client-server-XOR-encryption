# Assembly Echo Client-Server with XOR encryption 

An Echo client-server with XOR encryption for secured communication build with **Assembly** and **NASM**.

## Usage

1. Compile client and server:
```zsh
nasm -f elf64 -g serverXOR.asm
ld -static -o server serverXOR.o
```
```zsh
nasm -f elf64 -g clientXOR.asm
ld -static -o server clientXOR.o
```

2. Run the server and the client in seperate terminals. Now you can send encrypted message from client to server.
```zsh
./server
```
```zsh
./client
```
