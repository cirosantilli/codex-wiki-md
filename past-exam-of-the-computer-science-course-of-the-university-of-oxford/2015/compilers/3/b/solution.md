<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The useful repeated [program expressions](../../../../../program-expression.md), nested inside one another, are the [memory address](../../../../../memory-address.md) of `a[i]`, its value, and the [memory address](../../../../../memory-address.md) of `a[a[i]]`. Materialize each maximal reusable tree at the level at which it is shared, using fresh [temporary variables](../../../../../temporary-variable.md) `u`, `v`, and `w`:

```
MOVE(R(u), ADD(C(A),SHL(M(ADD(R(fp),C(I))),2)))
MOVE(R(v), M(R(u)))
MOVE(R(w), ADD(C(A),SHL(R(v),2)))
MOVE(R(t), M(R(w)))
MOVE(M(R(w)), R(v))
MOVE(M(R(u)), R(t))
```

Thus `u` is a saved [memory address](../../../../../memory-address.md), `v` the old [integer](../../../../../integer-split.md) value of `a[i]`, `w` the second saved [memory address](../../../../../memory-address.md), and `t` the old value at that second location. The two large address trees occur both in loads and as store destinations. After extracting them, the repeated load of `a[i]` inside the second address and as the middle assignment's source becomes `v`. Extracting every smaller nested tree again would add no benefit.

The relevant [alias analysis](../../../../../alias-analysis.md) facts are that local `i` does not occupy any location written through global `a`, that [frame pointer](../../../../../frame-pointer.md) `fp` and base $A$ stay fixed, and that `t,u,v,w` are distinct [processor registers](../../../../../processor-register.md) or otherwise nonoverlapping [temporary variables](../../../../../temporary-variable.md). There are no intervening calls, [volatile memory accesses](../../../../../volatile-memory-access.md), or concurrent changes. Under these assumptions, loading `i` once remains valid even across the array stores. Before the middle store, no array location has yet changed, so both its target [memory address](../../../../../memory-address.md) and its source value can be computed and saved earlier.

**No assumption that the two array locations are distinct is required.** The middle store may change `a[i]` when its target coincides with it, but `v` is not loaded again afterwards: only the saved address `u` is needed for the final store. It would be unsound to retain an arbitrary array load across an aliasing store and then treat it as the new contents; that is not what these trees do.

For a language with a true global [array](../../../../../array-data-structure.md), a distinct local variable, and no arbitrary means of fabricating [pointers](../../../../../pointer-computer-programming.md) to unrelated storage, these facts follow simply from declarations and the [stack frame](../../../../../stack-frame.md) layout. Accesses must denote valid [array](../../../../../array-data-structure.md) elements. In an unrestricted low-level language with overlapping storage, arbitrary [pointer](../../../../../pointer-computer-programming.md) arithmetic or unchecked out-of-range accesses, that conclusion requires extra guarantees. Omitting emitted [array bounds](../../../../../array-bounds.md) checks does not itself prove that all [memory addresses](../../../../../memory-address.md) are valid. If $M$ denotes a word load, the saved quantities are

$$
\boxed{u=A+(i\ll2),\quad v=M(u),\quad w=A+(v\ll2).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
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
