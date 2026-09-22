<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The printed lines are:

```
f with X at M
f with Y at N
f with Y at N
```

[Method overloading](../../../../../method-overloading.md) first uses static types. The receiver `m` has static type `M`, whose available signatures are `f(X)` and `f(Y)`. Argument `x` selects `f(X)`; `y` selects `f(Y)`; and `z`, statically `Z`, also selects `f(Y)` because that is the most specific available applicable signature. `N.f(Z)` is not available through the static receiver type.

Only after a signature is selected does [dynamic dispatch](../../../../../dynamic-dispatch.md) choose an override for the runtime receiver `N`. That class overrides `f(Y)` but not `f(X)`, explaining all three lines. The shared argument object's runtime class does not trigger a second overload-resolution pass.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
