# Questions

## What's `stdint.h`?

A C heade file that specifies specific fixed-width integer types, allowing interger types to stay consistent across different OS/architecture.

## What's the point of using `uint8_t`, `uint32_t`, `int32_t`, and `uint16_t` in a program?

Unsigned integers allow for greater number (double) of values to be assigned, as unsigned integers can only be positive and therfore 1 byte can have a value of 0 - 255, whereas a signed integer could have -127 - +127. uint8 indicates an 8 byte unsigned integer, therefore a value of up to (2 ^ 8)-1 can be assigned.

## How many bytes is a `BYTE`, a `DWORD`, a `LONG`, and a `WORD`, respectively?

BYTE = 1 byte (8bits), DWORD = 4 bytes (32 bit unsigned integer), LONG = 4 bytes (32bit signed integer), WORD = 2 bytes (16bit unsigned integer)

## What (in ASCII, decimal, or hexadecimal) must the first two bytes of any BMP file be? Leading bytes used to identify file formats (with high probability) are generally called "magic numbers."

Header file used to identify bitmap files ; B and M (ASCII), 0x42 and 0x4D (hex)

## What's the difference between `bfSize` and `biSize`?

bfSize is the size of the complete bitmap file in bytes; includes header files
biSize is fixed and is the size of the BITMAPINFOHEADER  file (which contains info about the image)

## What does it mean if `biHeight` is negative?

Indicates a top-down image, origin is upper left corner

## What field in `BITMAPINFOHEADER` specifies the BMP's color depth (i.e., bits per pixel)?

biBitCount

## Why might `fopen` return `NULL` in `copy.c`?

If the file does not exist or is not in the current directory

## Why is the third argument to `fread` always `1` in our code?

Always reading one x byte block

## What value does `copy.c` assign to `padding` if `bi.biWidth` is `3`?

TODO

## What does `fseek` do?

TODO

## What is `SEEK_CUR`?

TODO
