<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [overload selection followed by dynamic dispatch](../../../../../overload-selection-followed-by-dynamic-dispatch.md): the receiver's [static type](../../../../../static-type.md) determines visible signatures, and argument [static types](../../../../../static-type.md) choose the overload. The receiver's [runtime type](../../../../../runtime-type.md) then selects its override. A `super` call starts at the inherited implementation instead of redispatching to the override just entered.

For `c.f1(y)`, the `Y` overload is visible on `C`, so its body in `C` runs. For `a.f2(x)`, the `X` signature is selected and its override in `C` calls `C.f1(X)`. For `a.f2(y)`, the `Y` signature is selected; its body in `C` calls `super.f1(y)`. The superclass `B` has only `f1(X)`, so that call uses `B.f1(X)`.

For `b.f3(y)`, the [static type](../../../../../static-type.md) `B` exposes only `f3(X)`. Its override in `C` calls `super.f2(x)`, entering `B.f2(X)`. The unqualified `f1(x)` inside that body still uses [dynamic dispatch](../../../../../dynamic-dispatch.md) on the original `C` instance, so it calls `C.f1(X)`.

Finally `c.f4(x)` invokes the [companion object](../../../../../companion-object.md) `C`, which is a separate receiver extending `B`. Its `f3(X)` calls inherited `B.f2(X)`, whose `f1` call dispatches to `ObjC.f1(X)`.[p. 10, Question 6(a), method bodies and calls](../../../../../imperative-programming-examination-paper-by-the-university-of-oxford-2014.md)

The exact five output lines, including the final comma and space on each line, are:
```
f1(y:Y) in C, 
f1(x:X) in C, f2(x:X) in C, 
f1(x:X) in B, f2(y:Y) in C, 
f1(x:X) in C, f2(x:X) in B, f3(x:X) in C, 
f1(x:X) in ObjC, f2(x:X) in B, f3(x:X) in ObjC, f4(x:X) in C, 
```


$$
\boxed{\text{Select the signature statically, then dispatch that signature dynamically}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
