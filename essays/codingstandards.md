---
layout: essay
type: essay
title: Coding Standards are Important!
date: 2017-02-09
labels:
  - Coding standards

---



I think it is 

One thing that I am not so keen on in coding standards is restrictions on the number of lines in between lines of code. Especially since the opening braces are also supposed to be on the same line as the statement it applies to, rather than a line of its own, to me not allowing a space makes the code harder to digest.

That is, this:
```
const returntrue = function returntrue() {
    const returnfalse = function returnfalse() {
         return false;
    };
    return true;
}
```

is more difficult for me to digest than this:

```
const returntrue = function returntrue() {

    const returnfalse = function returnfalse() {

         return false;

    };

    return true;

}
```
