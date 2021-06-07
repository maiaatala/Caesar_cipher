# Caesar Cipher Program

Challenge resolved with the intent of training the use of strings in C language.
[link to the challenge page](https://www.reddit.com/r/dailyprogrammer/comments/myx3wn/20210426_challenge_387_easy_caesar_cipher/)

## Table of Contents

- [Caesar Cipher Program](#caesar-cipher-program)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [The logic](#the-logic)

***

## Introduction

The [program](caesar_cipher.c) was made with the intention of encrypting a text written by the user using the [Caesar's cipher method](https://en.wikipedia.org/wiki/Caesar_cipher)
on which each letter of the plaintext is replaced by another letter by advancing it some fixed positions down the alphabet, wrapping around form z back to a. For example:

> The caesar cipher of the letter `a` with **1** shift is `b`
> The caesar cipher of the letter `d` with **15** shift is `s`
> The caesar cipher of the plaintext `fusion` with **6** shift is `layout`

The program will accpet lowercase and uppercase letters and keep special characters (like: !,.;@#$%áú^) and spaces as is.

Programming language used: C

Program date: June 2021.

Made by: Ana C Maia Atala. :e-mail: @ ana.atala@unemat.br

***

## The logic

[The program](caesar_cipher.c) hasd the following basic logic steps:

1. The user will input their desired plaintext and what shift they want their text to be encrypted on.
2. The program will read the text as a string and scan it in a `for loop`.
    1. For each character in the string, the program will determine by using it's ASCII value if it is a lowercase, upercase or special character.
        1. If the char is a lowercase or uppercase letter, it will calculate the correct shifted letter and store it in the same position to the encrypted text string.
        2. If the char is a special char, it will be copied to the same position on the encrypted text string.
3. When the scan is over, it will print the stored plaintext and it's encrypted variation for the user.
