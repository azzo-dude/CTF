# Bit-O-Asm-1
- [Description](#Description)
- [Solution](#Solution)
## Description
```
Difficult: Medium

Can you figure out what is in the eax register? Put your answer in the
picoCTF flag format: picoCTF{n} where n is the contents of the eax
register in the decimal number base. If the answer was 0x11 your flag
would be picoCTF{17}.
```
Challenge link: [https://play.picoctf.org/practice/challenge/391?category=3&page=2]

## Solution

Bước đầu tiên ta sẽ tải và mở assembly dump, ta có đoạn text như sau:
```
<+0>:     endbr64 
<+4>:     push   rbp
<+5>:     mov    rbp,rsp
<+8>:     mov    DWORD PTR [rbp-0x4],edi
<+11>:    mov    QWORD PTR [rbp-0x10],rsi
<+15>:    mov    eax,0x30
<+20>:    pop    rbp
<+21>:    ret
```
