<h1 id="2/vi/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First derive the intersection constraints. Since $D$ is [nef](../../../../../../../nef-line-bundle.md) and $F,M$ are effective, $D\cdot F,D\cdot M\geq0$; their sum is $D^2=0$, so both vanish. Since the [movable divisor](../../../../../../../movable-part-of-a-linear-system.md) $M$ is nef, $M^2,M\cdot F\geq0$, and $M\cdot D=0$ forces both to vanish. In particular

$$
D\cdot F=D\cdot M=M^2=M\cdot F=F^2=0.
$$

For every component $E$ of $F$, nefness and $D\cdot F=0$ imply $D\cdot E=0$. The [isotropic orthogonality consequence of the Hodge index theorem](../../../../../../../isotropic-orthogonality-consequence-of-the-hodge-index-theorem.md) gives $E^2\leq0$. If $E^2=0$, [Riemann–Roch theorem for algebraic surfaces](../../../../../../../riemann-roch-theorem-for-algebraic-surfaces.md) and [Serre duality](../../../../../../../serre-duality.md) give $h^0(X,E)\geq2$, since $-E$ cannot be effective. Choose $E'\in|E|$ different from $E$. It cannot contain $E$: otherwise $E'-E$ would be a nonzero effective numerically trivial divisor, contradicting its positive intersection with an ample divisor. Choose a member of $|M|$ avoiding $E$. Replacing one copy of $E$ in $F$ by $E'$ now produces a member of $|D|$ with smaller multiplicity along $E$, contradicting the definition of the [fixed part](../../../../../../../fixed-part-of-a-linear-system.md). Therefore

$$
\boxed{E^2<0\quad\text{for every component of }F.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Vi](../../vi.md)
3. [2](../../../2.md)
4. [Paper 139](../../../../paper-139-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
