<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The five printed lines, including the comma and space after every fragment, are:
```
f1 in C, 
f1 in C, f2 in B, 
f1 in C, f2 in A, f3 in B, 
f1 in A, f2 in A, f3 in ObjB, f4 in B, 
f1 in ObjC, f2 in A, f3 in B, f4 in ObjC, f5 in C, 
```
[Scala](../../../../../scala.md) [dynamic dispatch](../../../../../dynamic-dispatch.md) uses the receiver's runtime [software class](../../../../../class-programming.md), even though `a` has the [static type](../../../../../static-type.md) `A`. Thus `a.f1` uses `C.f1`, and `a.f2` uses `B.f2` whose unqualified `f1` still dispatches on the `new C` receiver.

For `a.f3`, `B.f3` explicitly selects `super.f2`, which is `A.f2`. Inside `A.f2`, the unqualified call to `f1` still dispatches to `C.f1`; `super` does not replace the receiver. For `a.f4`, `B.f3` in the body of class `B` means a call on the [singleton object](../../../../../singleton-object.md) `B`, not on `this`. That object's `f3` calls `A.f2`, which calls `A.f1`.

Finally `a.f5` calls `C.f4` on the [singleton object](../../../../../singleton-object.md) `C`. That object extends class `B`, overrides `f1` and `f4`, and inherits class `B`'s `f3`. Its `f4` calls this inherited `f3`; that selects `A.f2`, whose `f1` dispatches to the object's own override. These distinctions follow member selection and `super` semantics.[This and Super; Designators, member selection](../../../../../scala-2-11-expressions-specification.md)

$$
\boxed{\text{Ordinary calls keep the receiver; explicit B and C name their singleton objects}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
