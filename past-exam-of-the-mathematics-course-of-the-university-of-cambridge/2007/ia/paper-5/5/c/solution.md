<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If `f : 'a -> 'b`, then the success constructor applied to `f x` has type `'b result`, and the exception alternative has that same type. Therefore
```
what : ('a -> 'b) -> 'a -> 'b result
```
The zero comparison fixes the labels to type `int`, and `tony` with this predicate accepts an `int tree` and normally produces a Boolean. The requested expression consequently has type
```
int tree -> bool result
```
so **the wrapper maps an integer tree to a packaged Boolean result or exception packet**.

For `ta`, the packet `Ian true` means that a normal successful search occurred: `ta` has at least one root-to-`Lf` path all of whose branch labels are nonzero. It can be `Lf`; if nonempty, its root must be nonzero, but labels away from the successful path need not be. For example, `Br(1,Lf,Br(0,Lf,Lf))` succeeds despite containing a zero.

For `tb`, `Cherie Blair` means that the search raised the designated exception. Every root-to-`Lf` path has a zero-labeled branch somewhere. Thus `tb` is nonempty, but its root need not be zero: `Br(1,Br(0,Lf,Lf),Br(0,Lf,Lf))` fails. With the supplied total comparison predicate, `tony` can return only `true` or raise `Blair`, never return `false`. **`ta` admits an all-nonzero path; `tb` admits none.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
