<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the following explicit tree notation for the [intermediate representation](../../../../../intermediate-representation.md). `C(k)` is a constant, `R(r)` a [processor register](../../../../../processor-register.md), `M(e)` a word load from [memory address](../../../../../memory-address.md) `e`, `ADD` [addition](../../../../../addition.md), and `SHL(e,2)` a [left shift](../../../../../left-shift.md) by two [bits](../../../../../bit.md). `MOVE(destination,source)` assigns either a [processor register](../../../../../processor-register.md) or the [computer memory](../../../../../computer-memory-split.md) word designated by `M`. Parentheses show complete tree structure, so these displays specify trees rather than already shared [Directed acyclic graphs](../../../../../directed-acyclic-graph.md).

Let $A$ be the constant base [memory address](../../../../../memory-address.md) of the global [array](../../../../../array-data-structure.md) `a`, and $I$ the constant offset of local `i` from the [frame pointer](../../../../../frame-pointer.md) `fp`. Each [integer](../../../../../integer-split.md) occupies four [bytes](../../../../../byte.md), and array indices are zero-based; a fixed nonzero lower bound can instead be absorbed into $A$. Local `t` is represented by `R(t)`. After replacing [multiplication](../../../../../multiplication.md) by four with a [left shift](../../../../../left-shift.md), the three trees are:

```
MOVE(R(t),
     M(ADD(C(A),
           SHL(M(ADD(C(A),
                     SHL(M(ADD(R(fp),C(I))),2))),2))))

MOVE(M(ADD(C(A),
           SHL(M(ADD(C(A),
                     SHL(M(ADD(R(fp),C(I))),2))),2))),
     M(ADD(C(A),SHL(M(ADD(R(fp),C(I))),2))))

MOVE(M(ADD(C(A),SHL(M(ADD(R(fp),C(I))),2))),
     R(t))
```

Every `M(ADD(R(fp),C(I)))` loads `i`; the next enclosing `M` loads `a[i]`; the outermost `M` in the first tree loads `a[a[i]]`. **Each [array](../../../../../array-data-structure.md) index is converted to a [byte](../../../../../byte.md) offset by a [left shift](../../../../../left-shift.md) of two [bits](../../../../../bit.md).** The address rule used in all three trees is

$$
\boxed{\mathrm{addr}(a[k])=A+(k\ll 2)=A+4k.}
$$

 The source language's [array bounds](../../../../../array-bounds.md) checks are omitted as requested.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Compilers](../../../compilers-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
