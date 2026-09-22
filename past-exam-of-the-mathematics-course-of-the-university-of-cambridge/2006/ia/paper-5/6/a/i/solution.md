<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

These [Standard ML](../../../../../../../standard-ml.md) declarations separate the three evaluation and mutation models:
```
sml
datatype 'a olist = ONil | OCons of 'a * 'a olist;

datatype 'a lnode = LNil | LCons of 'a * (unit -> 'a lnode);
type 'a llist = unit -> 'a lnode;

datatype 'a mnode = MNil | MCons of 'a * 'a mnode ref;
type 'a mlist = 'a mnode ref;
```
The ordinary [linked list](../../../../../../../linked-list.md) is immutable and its spine is built eagerly. A [lazy list](../../../../../../../lazy-list.md) is a delayed function producing the next constructor, with another delayed function for its tail; it can describe an infinite stream without constructing it in advance. A [mutable list](../../../../../../../mutable-list.md) uses an [ML reference type](../../../../../../../ml-reference-type.md) cell for both the root link and every tail link. Updating those cells can remove nodes, including the original head. This [lazy list](../../../../../../../lazy-list.md) representation delays evaluation but does not automatically implement [memoization](../../../../../../../memoization.md); repeated forcing can repeat work or effects.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
