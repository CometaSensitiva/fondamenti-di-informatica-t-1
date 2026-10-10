# Fondamenti di Informatica T-1 · C

**English** · [Italiano](README.it.md)

A small C library and an exam starter kit I wrote for *Fondamenti di Informatica T-1* at the University of Bologna (Computer Engineering, 2022–23). It was my first contact with programming and with GitHub. Part of my [university work](https://github.com/CometaSensitiva/university).

## What's inside

| Folder | Contents |
| --- | --- |
| [`Libreria/`](Libreria) | Generic element type with compare/assign/swap, dynamic arrays, sorting algorithms (naive, bubble, insertion, merge, quick sort) and a linked-list ADT |
| [`Esame/`](Esame) | An empty exam template with source files, sample data and placeholders for four exercises |

The library is written around a replaceable element type (`myType`, `mySecondType`), so the same sorting and list functions work for the records of each exam text.

## Use it

For the exam template, create an empty C project in Visual Studio and add the `.c` and `.h` files from **Esame only**. Keep `file1.txt` and `file2.txt` in the program's working directory. `main.c` contains placeholders, not a completed exam solution.

With Clang or GCC, from the repository root:

```sh
cc -std=c11 Esame/*.c -o /tmp/esame
(cd Esame && /tmp/esame)
```

`Libreria` is a separate collection to adapt to an exercise. Do not combine both folders in one executable: they contain overlapping utility definitions. The historical library also needs header/type setup, and its custom `srand48` declaration conflicts with the system declaration on macOS and Linux.
