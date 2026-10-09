# Fondamenti di Informatica T-1 · C

**English** · [Italiano](README.it.md)

A small C library and an exam starter kit I wrote for *Fondamenti di Informatica T-1* at the University of Bologna (Computer Engineering, 2022–23). It was my first contact with programming and with GitHub. Part of my [university work](https://github.com/CometaSensitiva/university).

## What's inside

| Folder | Contents |
| --- | --- |
| [`Libreria/`](Libreria) | Generic element type with compare/assign/swap, dynamic arrays, sorting algorithms (naive, bubble, insertion, merge, quick sort) and a linked-list ADT |
| [`Esame/`](Esame) | The library applied to a past exam text: file reading, list handling and the structure of a typical solution |

The library is written around a replaceable element type (`myType`, `mySecondType`), so the same sorting and list functions work for the records of each exam text.

## Use it

The starter kit was built for Visual Studio on Windows, which the course used. Copy the `.c` and `.h` files of both folders into an empty project, keeping `Libreria` and `Esame` as two filters, and build `Esame/main.c`. The step-by-step guide is in the [Italian README](README.it.md#come-usarlo).
