---
layout: page
title: Bengali Programming Language
description: Designing a compiled programming language with Bengali syntax for K-12 students
img: assets/img/projects/bangla_compiler.jpg
importance: 2
category: coursework
---

About 99.8% of secondary students in Bangladesh learn in Bengali, yet every mainstream teaching language (C, Python, Scratch) uses English keywords. Existing Bengali languages such as ChaScript and Pankti are interpreted and dynamically typed. We set out to design a **compiled, statically typed language with fully Bengali syntax** for school students.

- **Grammar:** defined the language in BNF, modelled on C: variables, conditionals (যদি … তাহলে … নয়তো), loops (যতক্ষন), functions (ফাংশন) and Bengali numerals.
- **Lexer and parser:** built on LLVM's Kaleidoscope tutorial in C++. The lexer reads Unicode Bengali characters with `wchar_t`/`wstring` and converts Bengali digits; the parser builds an abstract syntax tree and prints its output in Bengali in the terminal.
- **Backend:** LLVM identifiers only accept narrow characters, so we wrote a reverse/forward phonetic map between Bengali and ASCII. Full code generation to machine code remained unsolved and is the next step.

{% include figure.liquid loading="eager" path="assets/img/projects/bangla_compiler.jpg" title="Bengali syntax" class="img-fluid rounded z-depth-1" zoomable=true %}

<div class="caption">A sample program in the designed syntax: a function, a conditional and a loop.</div>

Course project (CSE 425), North South University, Fall 2024 · Noman Saffat Sajid, Moshiur Rahman, Maisha Subha, Shahariar Ifti · C++, LLVM
