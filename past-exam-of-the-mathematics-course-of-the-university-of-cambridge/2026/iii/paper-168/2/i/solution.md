<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Decompose $f=\sum_{j=0}^n f^{(=j)}$ into its homogeneous [Fourier levels](../../../../../../fourier-walsh-transform.md). The [Bonami lemma](../../../../../../bonami-lemma.md) and the [triangle inequality](../../../../../../triangle-inequality.md) give

$$
\lVert T_{1/\sqrt3}f\rVert_4
\leq\sum_j3^{-j/2}\lVert f^{(=j)}\rVert_4
\leq\sum_j\lVert f^{(=j)}\rVert_2
\leq\sqrt{n+1}\,\lVert f\rVert_2.
$$

Apply this estimate to the $m$-fold tensor power $f^{\otimes m}$. Tensor products multiply both relevant norms and commute with the [noise operator on the Boolean hypercube](../../../../../../noise-operator-on-the-boolean-hypercube.md), so

$$
\lVert T_{1/\sqrt3}f\rVert_4^m
\leq\sqrt{mn+1}\,\lVert f\rVert_2^m.
$$

Taking $m$th roots and the [limit](../../../../../../limit-of-a-function.md) $m\to\infty$ proves the [hypercontractive inequality on the Boolean hypercube](../../../../../../hypercontractive-inequality-on-the-boolean-hypercube.md)

$$
\lVert T_{1/\sqrt3}f\rVert_4\leq\lVert f\rVert_2.
$$

The noise operators are self-adjoint and satisfy $T_\rho T_\sigma=T_{\rho\sigma}$. By the [duality of Lp spaces](../../../../../../duality-of-lp-spaces.md),

$$
\lVert T_{1/\sqrt3}f\rVert_2
=\sup_{\lVert g\rVert_2=1}|\langle f,T_{1/\sqrt3}g\rangle|
\leq\lVert f\rVert_{4/3}.
$$

Consequently

$$
\boxed{\operatorname{Stab}_{1/3}(f)
=\langle f,T_{1/3}f\rangle
=\lVert T_{1/\sqrt3}f\rVert_2^2
\leq\lVert f\rVert_{4/3}^2.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
