<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A computed [memory address](../../../../../memory-address.md) is just another [integer](../../../../../integer-split.md) on the operand [stack](../../../../../stack-data-structure.md). For a [pointer](../../../../../pointer-computer-programming.md) held at fixed address $p$, `const p; load` obtains the pointed-to address; another `load` obtains its contents. More generally, any expression that leaves an address on top may be followed by `load`, or may be retained beneath a computed value for `store`.

For an [array](../../../../../array-data-structure.md) whose base address is $b$ and whose element size is $w$ address units, the address of entry $i$ is $b+wM[p_i]$, where $p_i$ stores the index. Add [zero-address instructions](../../../../../zero-address-instruction.md) `mul` and `dup`, with `dup` mapping $S,p$ to $S,p,p$. A suitable sequence is
```
const b
const p_i
load
const w
mul
add
dup
load
const 1
add
store
```
The first six instructions leave the element address $p=b+wM[p_i]$. The remaining suffix evolves as

$$
S,p\longmapsto S,p,p\longmapsto S,p,M[p]\longmapsto S,p,M[p],1\longmapsto S,p,M[p]+1\longmapsto S,
$$

with the final effect

$$
\boxed{M[b+wM[p_i]]\gets M[b+wM[p_i]]+1.}
$$

The address is computed once and duplicated, so both accesses refer to the same [array](../../../../../array-data-structure.md) element. For unit-sized elements omit `const w; mul`. If the base address is itself held in a variable, replace `const b` by the instructions loading that variable's value. No instruction other than `const` requires an explicit operand.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
