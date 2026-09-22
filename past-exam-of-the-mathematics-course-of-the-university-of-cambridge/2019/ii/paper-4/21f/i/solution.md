<h1 id="21f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose $\phi^3=\operatorname{Id}_X$. Since $\phi$ has no fixed points, neither does $\phi^2$: if $\phi^2(x)=x$, then applying $\phi$ gives $\phi(x)=\phi^3(x)=x$. The Lefschetz theorem therefore gives

$$
L(\phi)=L(\phi^2)=0,
\qquad
L(\operatorname{Id}_X)=\chi(X)=n.
$$

For each $q$, the averaging operator

$$
P_q=\frac13\left(I+\phi_*+\phi_*^2\right)
$$

is the projection of $H_q(X;\mathbb Q)$ onto its $\langle\phi\rangle$-invariant subspace, so its trace is an integer. Taking the alternating sum of these traces gives

$$
\sum_q(-1)^q\operatorname{tr}P_q
=\frac13\{L(\operatorname{Id}_X)+L(\phi)+L(\phi^2)\}
=\frac n3.
$$

The left side is an integer. By [Euler-characteristic divisibility from a fixed-point-free cyclic action](../../../../../../euler-characteristic-divisibility-from-a-fixed-point-free-cyclic-action.md),

$$
\boxed{3\mid n.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [21F](../../21f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
