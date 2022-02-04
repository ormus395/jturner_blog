---
title: LISP!
date: 2022-02-03
description: A short introduction to Lisp
---

### What is Lisp?

Lisp is a programming language that was developed in 1958 by a man named John McCarthy. McCarthy developed the language while he was attending MIT. The language is fully parenthesized and loosely follows the syntax of Lamda Calculus.

Lisp has developed several dialects over the ages, and the one that will be briefly covered in this article will be Scheme.

## The syntax

Like Lisp, Scheme is a fully parenthesized language that loosely follows the syntax of Lambda Calculus.

```
(thing (thing2) (thing3) (thing4))
```

In Lisp, everything encased in parenthesis is considered a procedure.
Be it arithmetic, defining a function, or developing branching, every _thing_ must be encased in parenthesis.

```
((so) (many) (parenthesis))
```

## Arithmetic

Arithmetic in Scheme is prefix notation. 
What is prefix notation besides _annoying_?
Prefix notation is where the operator is before the operands. 

```
; to do addition, the plus operator must go before the operands
(+ 3 2)

; this is the case with all types of arithmetic operations
(* 4 3)

; division
(/ 4 5)

; now we're getting hairy
(> 3 4)
```

### That's all for not folks

In an edit to this article, I'll be going over function definitions and branching. Further down the road recursion will also be covered. Thanks for reading!