<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [ML reference type](../../../../../../ml-reference-type.md) `'a ref` describes a mutable cell holding a value of type `'a`. The operations are `ref : 'a -> 'a ref` for allocation, `! : 'a ref -> 'a` for dereferencing and `:= : 'a ref * 'a -> unit` for assignment. An immutable variable binding can name a mutable cell; assigning to the cell does not change what the binding denotes. Two names may alias the same cell, so an update through either is visible through the other.
```
val counter = ref 0;
val alias = counter;
counter := !counter + 1;
```
Both dereferences now give one. A reference's stored type remains fixed; the value restriction prevents allocating one unrestricted polymorphic cell and then using incompatible instantiations.

[Imperative programming](../../../../../../imperative-programming.md) uses sequencing `(e1; e2; ...; en)` to perform effects left to right, with the final expression supplying the result. Conditional expressions choose one branch. `while condition do body` repeatedly checks a Boolean condition and performs a unit-valued body, returning `()` on termination. [Standard ML](../../../../../../standard-ml.md) has no required primitive `for` loop, but recursion or a reference with `while` supplies one. For example:
```
fun sumTo n =
    let val i = ref 1
        val total = ref 0
    in
        while !i <= n do
          (total := !total + !i; i := !i + 1);
        !total
    end;
```
**References provide mutable state; sequencing, conditionals and loops control its updates.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
