<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The hypotheses make $p$ a [sublinear functional](../../../../../../sublinear-function.md) and $q$ a [superlinear functional](../../../../../../superlinear-functional.md). In particular $p(0)=q(0)=0$. Apply the domination property to $y+y'\in Y$ and the vector $x+x'$:

$$
S(y)+S(y')\leq p(x+x'+y+y')-q(x+x').
$$

[Subadditivity](../../../../../../subadditive-sequence.md) of $p$, with the inserted vectors $z$ and $-z$, gives

$$
p(x+x'+y+y')\leq p(x+y+z)+p(x'+y'-z).
$$

Superadditivity of $q$ gives $q(x+x')\geq q(x)+q(x')$. Combining these inequalities and moving terms yields exactly

$$
\boxed{S(y')-p(x'+y'-z)+q(x')
\leq-S(y)+p(x+y+z)-q(x).}
$$

Every vector appearing in the comparison is permitted by the assumed domination, so no membership of $x,x',z$ in $Y$ is needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
