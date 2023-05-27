# Dependecies


![lol](https://raw.githubusercontent.com/khrome/ansi-gif/HEAD/Samples/nyan.gif)

    section .data
        hello db 'Hello, World!', 0

    section .text
        global _start

    _start:
        ; Write the string to stdout
        mov eax, 4       ; System call number for write
        mov ebx, 1       ; File descriptor for stdout
        mov ecx, hello   ; Address of the string
        mov edx, 13      ; Length of the string
        int 0x80         ; Call the kernel

        ; Exit the program
        mov eax, 1       ; System call number for exit
        xor ebx, ebx     ; Exit code 0
        int 0x80         ; Call the kernel
