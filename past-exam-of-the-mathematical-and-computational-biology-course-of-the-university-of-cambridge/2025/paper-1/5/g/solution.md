<h1 id="5/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Suppose $r>1$ and set $q=\log r/(r-1)$. Substitution of the positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) into the [Jacobian matrix](../../../../../jacobian-matrix.md) gives

$$
J_*=
\begin{pmatrix}
1&-r\log r/[b(r-1)]\\
b(r-1)/r&q
\end{pmatrix},\quad
\operatorname{tr}J_*=1+q,\quad
\det J_*=q+\log r=\frac{r\log r}{r-1}.
$$

Part (b) showed $f(x)<0$ whenever $x\ne1$. In particular,

$$
f(1/r)=\frac{1-r+\log r}{r}<0
$$

gives $\log r<r-1$, whereas

$$
f(r)=r-1-r\log r<0
$$

gives $\det J_*>1$. The latter already violates the [Jury stability criterion](../../../../../jury-stability-criterion.md) condition $1-\det J_*>0$. More directly, the product of the two [eigenvalues](../../../../../eigenvalue.md) is greater than one, so at least one has [modulus](../../../../../modulus.md) greater than one. Therefore the positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) is **unstable**. This is the [instability of the Nicholson-Bailey equilibrium](../../../../../instability-of-the-nicholson-bailey-equilibrium.md); parasitoid feedback in this simple model does not stabilize coexistence.

## ↑ Ancestors (13)

1. [G](../g.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
