<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Method overloading](../../../../../method-overloading.md) chooses a signature using the [static types](../../../../../static-type.md) available at the call site. The receiver `m` has [static type](../../../../../static-type.md) `M`, whose visible overloads accept `X` and `Y`; the `Z` overload introduced only in `N` is not a candidate.

For `m.f(x)`, the argument's [static type](../../../../../static-type.md) is `X`, so the chosen signature is `f(X)`. `N` does not override it, and the inherited `M` body runs. For `m.f(y)`, the chosen signature is `f(Y)`, and [dynamic dispatch](../../../../../dynamic-dispatch.md) on the receiver chooses `N`'s override. For `m.f(z)`, both visible signatures apply, but `f(Y)` is more specific than `f(X)`. [Dynamic dispatch](../../../../../dynamic-dispatch.md) again chooses `N.f(Y)`. Thus
```
f with X at M
f with Y at N
f with Y at N
```
Equivalently,

$$
\boxed{X@M,\qquad Y@N,\qquad Y@N.}
$$

The [runtime type](../../../../../runtime-type.md) of every argument is `Z`, but ordinary single-receiver [dynamic dispatch](../../../../../dynamic-dispatch.md) does not redo [method overloading](../../../../../method-overloading.md) using that [runtime type](../../../../../runtime-type.md). This is [overload selection followed by dynamic dispatch](../../../../../overload-selection-followed-by-dynamic-dispatch.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
