---
layout: essay
type: essay
title: "TypeScript (Almost) Saves the Internet"
# All dates must be YYYY-MM-DD format!
date: 2025-09-03
published: true
labels:
  - TypeScript
  - JavaScript
  - Static Typing
---

<img class="img-fluid" src="../img/ts-logo-256.png">

## On Dynamic Typing

Dynamic typing sucks. I know that this take may not be the most popular, but if there were one computer science hill to die on, it would be that. Dynamic typing is just too loose. What do you mean, I can pass an object in place of a number? That shouldn’t be allowed! I need structure and clarity in my code, but dynamic typing creates the possibility for so many bugs that aren’t caught at compile time. Fortunately, the solution is simple: just use a statically typed language.

## Typescript

JavaScript is the programming language of the Internet. It is used everywhere because it has to be, as one of the few languages web browsers can parse. To my dismay, it is dynamically typed, but I don’t fret because there is a solution: Typescript. TypeScript is a superset of JavaScript, adding many features that its predecessor desperately needs. On top of that, the good features of JavaScript are a boon to TypeScript, though this comes with the curse of JavaScript’s problems as well. But first, Typescript’s successes:

### 1) Static Typing

As I’ve said before, static typing is amazing. It contributes greatly to code clarity and maintainability.

### 2) Access Modifiers

JavaScript does not have access modifiers (`public`, `private`, etc.) while TypeScript does. I believe this to be a huge oversight, because to me, classes in OOP should allow engineers to store and manage state while maintaining certain invariants. The ability to mutate internal state from an external source poses a real problem for such invariants, making access modifiers a welcome feature of Typescript.

### 3) Anonymous Functions

Don’t think that because I like the improved OOP support of Typescript, that I dislike functional programming. Support for the functional programming paradigm is also a great feature (though we can thank JavaScript for this one). The ability to assign functions to variables and return them from other functions enables greater code reusability and array utility methods such as `map()`, `find()`, and `reduce()`.

## Things I Would Change about Typescript

I do think TypeScript is a good programming language. It succeeds in adding extra code clarity and compile-time type checking to JavaScript, to help maintain more sustainable code. However, it is not without its flaws (and I have my preferences too).

### 1) Typescript Must be Compiled

I understand that this is by no fault of TypeScript (I blame the misguided programmers who decided long ago that JavaScript would forever be the language of the internet), but having to transpile into an interpreted language seems inefficient. Browsers are designed to parse and run JavaScript at runtime, so why not enable them to parse TypeScript too? Surely static typing would contribute to speed.

### 2) Silent “Failures”

When code is not valid Typescript but is valid JavaScript, it is still compiled. If there is a problem that I or my linter didn’t catch, my compiler should catch it, not ignore it and move on. You can disable this behavior, but it’s on by default.

### 3) Hoisting

Yes, yet another problem with JavaScript that catches Typescript out. Contrary to what JavaScript allows, you shouldn’t be able to use variables outside of their scope. There is always a cleaner way of writing your code that doesn’t involve hoisting. The `var` keyword is merely a thorn in the foot of any developer unlucky enough to stumble onto it.

## Wrap Up

I view TypeScript as an amazing programming language created to fix a poorer one. I believe many of its flaws would have been avoided had it not been built as a superset of JavaScript, which forced it to inherit the mistakes that JavaScript made. At the same time, though, it being a layer on top of JavaScript allows it to be ubiquitously used across the internet, for better or worse.
