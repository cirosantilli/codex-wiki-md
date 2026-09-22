<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The irreducible finite-dimensional [unitary representations](../../../../../../unitary-representation.md) of $SU(2)$ are $E_n=\operatorname{Sym}^n(\mathbb C^2)$, one for each $n\geq0$, with dimension $n+1$. Equivalently they are spin-$j$ representations with $j=n/2$. The defining representation has $n=1$, and $n=0$ is trivial. Every finite-dimensional [unitary representation](../../../../../../unitary-representation.md) is an orthogonal [direct sum](../../../../../../direct-sum.md) of these.

Choose self-adjoint angular-momentum generators $J_x,J_y,J_z$ with $[J_x,J_y]=iJ_z$ cyclically. The actual [SU(2) Lie algebra](../../../../../../su-2-lie-algebra.md) generators are $L_a=-iJ_a$, so $[L_x,L_y]=L_z$. On an orthonormal weight basis $v_m$, $m=-j,-j+1,\ldots,j$, the complexified action is

$$
J_zv_m=mv_m,\qquad
J_\pm v_m=\sqrt{(j\mp m)(j\pm m+1)}\,v_{m\pm1},\quad J_\pm=J_x\pm iJ_y.
$$

The [Casimir operator](../../../../../../casimir-element.md) in this normalization is $C=-\sum_aL_a^2=\sum_aJ_a^2$, acting by

$$
\boxed{C|_{E_n}=j(j+1)I=\frac{n(n+2)}4I.}
$$

Other Lie-algebra metric normalizations rescale this scalar. On the diagonal subgroup $\operatorname{diag}(e^{it},e^{-it})$, the weights of $E_n$ are $n,n-2,\ldots,-n$, all with multiplicity one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
