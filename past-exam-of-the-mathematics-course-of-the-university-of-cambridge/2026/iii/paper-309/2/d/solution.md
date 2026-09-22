<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

After the trace gauge, $h_{ab}=\bar h_{ab}=A_{ab}e^{ik\cdot x}$. The [linearized Riemann curvature operator](../../../../../../linearized-riemann-curvature-operator.md) is built from terms containing two factors of $k$ and one factor of $A$:

$$
R^{(1)}_{abcd}
=-\frac12\left(
k_c k_bA_{ad}+k_d k_aA_{bc}
-k_d k_bA_{ac}-k_c k_aA_{bd}
\right)e^{ik\cdot x}.
$$

Contracting with $k^{[c}v^{d]}$ gives zero by $k^2=0$ and $k^aA_{ab}=0$, so $\mathcal R(k\wedge v)=0$. If $\omega_{cd}k^d=0$, every term in $R^{(1)}_{ab}{}^{cd}\omega_{cd}$ also contains such a contraction and vanishes.

To count the kernel, use the null basis $k,\ell,e_1,e_2$. The forms $k\wedge v$ span the three-dimensional space

$$
\langle k\wedge\ell,\ k\wedge e_1,\ k\wedge e_2\rangle.
$$

The condition $\omega_{ab}k^b=0$ defines the three-dimensional space

$$
\langle k\wedge e_1,\ k\wedge e_2,\ e_1\wedge e_2\rangle.
$$

Their intersection has dimension two, so their sum is a four-dimensional subspace of $\ker\mathcal R$. Since $\dim\Lambda^2=6$, the rank-nullity theorem gives

$$
\boxed{\operatorname{rank}\mathcal R\leq2.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
