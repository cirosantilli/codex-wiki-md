<h1 id="11h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The continued-fraction algorithm gives

$$
\sqrt{11}=3+\frac{\sqrt{11}-3}{1},\qquad
\frac1{\sqrt{11}-3}=\frac{\sqrt{11}+3}{2},\qquad
\frac1{(\sqrt{11}+3)/2-3}=\sqrt{11}+3,
$$

after which the process repeats. Thus

$$
\boxed{\sqrt{11}=[3;\overline{3,6}]}.
$$

The first two convergents are $3/1$ and $10/3$, of [field norms](../../../../../../field-norm.md) $-2$ and $1$ respectively. The even period gives the fundamental solution

$$
\boxed{x=10,\qquad y=3}.
$$

It is also directly the smallest positive solution: for $y=1,2$, the values $1+11y^2$ are $12,45$, neither square; $y=3$ gives $100$. Cubing by the preceding [Pell equation](../../../../../../pell-equation.md) group law gives

$$
\boxed{(10,3)^{\circ3}=(3970,1197)}.
$$

Indeed $3970^2-11\cdot1197^2=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11H](../../11h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
