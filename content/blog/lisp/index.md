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

## Defining Functions

Functions are the fundemental building block of functional programming. A good way of thinking about what a function in Scheme or any other programming language is the mathematical function. 

A function in math takes an argument: like x, and does a procedure or operation, x + 2, and returns the value from the operation. In computer programming, a function is just like that, but computer programming functions are not bound to just numbers.

For example, in Scheme, you can creat a function that determines what type of Igneas rock you have.

```
; First, we need to use the define keyword to create the function
(define (functionName value value value)
    ; this would be the function body
)
```

If you noticed, we used the keyword _define_ to tell Scheme we're going to be creating a function. Followed by a parenthesis, inside the parathesis is the function name, followed by the parameters of the function.
Also notice each function parameter is sperated not by commas, like other programming langauges, but by spaces.

Lets continue defining our igneas function.
```
(define (igneas darkMin)
    ; cond is a keyword used for branching
    ; I'll cover types of branching in scheme later
    (cond
        ((< darkMin 35) "Leucocratic")
        ((< darkMin 65) "Mesocratic")
        ((< darkMin 90) "Melanocratic")
        (#t "Ultramafic")
    )
)
```

Notice how Scheme does not have a return statement. So what Does the above function return? Well, it implicitly returns a result from a procedure. In the case of the *igneas function* we have on expression for a procedure: the cond expression. The cond expression is a lot like the _switch case_ expression found in other languages. If you are unfamiliar with types of branching, stay tuned, because I will be covering it in another update.

To summarize functions in scheme, they're the basic building block of the program. They're created by using the _define_ keyword, take arguments and implicitly return the value from an expression.

## Stay tuned, an update more on function and branching will be coming!