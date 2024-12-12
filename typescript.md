## What is TypeScript?

TypeScript is a language that has all the same features and syntax as Javascript and behaves identically at runtime.
However, it adds a static type checker with the caveat that all types are erased at runtime to preserve the behaviour of javascript.
This is so that it is easy to transition between the languages without worrying about anything breaking.

## Javascript Vs TypeScript

Javascript has a number of strange quirks such as:
    - Allowing the referencing of non-existent properties
    - Its equality operator coercing operands
    - Math.min() is greater than Math.max()
    - The expression true + true + true evaluates to 3
    - NaN is not equal to NaN
    - Many, many more

Typescript will produce compiler errors alerting the author in the scenorios where a behaviour is technically legal within javascript but 
may produce unexpected/unwanted behaviour. 

## Target

Sometimes, the author might deploy their code to older environments.
In which case, the target setting allows the author to downlevel JS features to whichever version the author specifies.
The author may also choose to adjust for a higher target setting if they know that their code is fit to run in newer environments.
With target, code can be run in older or newer environments without having to rewrite it manually.
