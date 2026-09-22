<h1 id="6e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $ad\equiv bc\pmod n$ and choose $r,s$ as in part (b). Put $\lambda=rc+sd$. Multiplying $ra+sb\equiv1$ by $c$ and using $ad\equiv bc$ gives

$$
\lambda a=rac+sad\equiv rac+sbc\equiv c\pmod n.
$$

Similarly, multiplication by $d$ gives $\lambda b\equiv d\pmod n$.

Moreover, $\lambda$ is a [unit modulo n](../../../../../../unit-modulo-n.md): if a prime divided both $\lambda$ and $n$, the two congruences would make it divide $c,d,n$, contrary to $(c,d)\in Y$. Thus $R$ means precisely that two pairs differ by multiplication by a unit modulo $n$. Reflexivity, symmetry using $\lambda^{-1}$, and transitivity using products of units now show that $R$ is an [equivalence relation](../../../../../../equivalence-relation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
