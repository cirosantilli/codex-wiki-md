<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [overload selection followed by dynamic dispatch](../../../../../overload-selection-followed-by-dynamic-dispatch.md): [method overloading](../../../../../method-overloading.md) chooses a signature from the receiver's [static type](../../../../../static-type.md) and argument [static types](../../../../../static-type.md), then [dynamic dispatch](../../../../../dynamic-dispatch.md) chooses an override of that signature using the receiver's [runtime type](../../../../../runtime-type.md). A `super` call selects the inherited implementation; a call on the [companion object](../../../../../companion-object.md) `B` uses that object's own methods.[Static overload resolution; this and super](../../../../../scala-2-11-expressions-specification.md)

The output, in order, is
```
f(x:X) in B
f(y:Y) in A
f(x:X) in A, g(x:X) in B
f(x:X) in ObjB, g(y:Y) in ObjB, h(y:Y) in B, h(z:Z) in C
f(y:Y) in C, m(a:A) in Y, k(x:X) in C
```
For `a.f(x)`, the argument's [static type](../../../../../static-type.md) is `X`, selecting `f(X)`; the receiver's [runtime type](../../../../../runtime-type.md) `B` selects `B.f(X)`. For `a.f(z)`, the receiver's [static type](../../../../../static-type.md) `A` exposes only `f(X)` and `f(Y)`. The `Z` argument fits both, and `f(Y)` is more specific. `B` does not override that signature, so `A.f(Y)` runs. The additional overload `B.f(Z)` is invisible through `a`.

For `c.g(z)`, the inherited instance `B.g(X)` calls `super.f(x)`, which is `A.f(X)`. For `c.h(z)`, [method overloading](../../../../../method-overloading.md) selects `C.h(Z)`. Its `super.h(z)` calls `B.h(Y)`, where the local parameter has [static type](../../../../../static-type.md) `Y`. Consequently `B.g(y)` selects `g(Y)` on the [companion object](../../../../../companion-object.md), whose only `f` signature is `f(X)`.

Finally, `c.k(x)` calls `x.m(this)`. The receiver `x` has [runtime type](../../../../../runtime-type.md) `Y`, so [dynamic dispatch](../../../../../dynamic-dispatch.md) enters `Y.m(A)`. Inside that method, `this` has [static type](../../../../../static-type.md) `Y`, selecting `a.f(Y)`; the actual argument object is `c`, so [dynamic dispatch](../../../../../dynamic-dispatch.md) reaches `C.f(Y)`. Therefore

$$
\boxed{\texttt{c.k(x)}\text{ produces }\texttt{f(y:Y) in C, m(a:A) in Y, k(x:X) in C}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
