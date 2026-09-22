<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the paper's convention, $\dot h_{ij}=2NK_{ij}+D_iN_j+D_jN_i$. The [Legendre transform in mechanics](../../../../../../legendre-transform-in-mechanics.md) therefore gives

$$
H=\int d^3x\left[\sqrt hN(K_{ij}K^{ij}-K^2-{}^{(3)}R)+2\pi^{ij}D_iN_j\right].
$$

Indeed $\pi^{ij}K_{ij}=\sqrt h(K_{ij}K^{ij}-K^2)$, and inversion of the [canonical momentum of the spatial metric](../../../../../../canonical-momentum-of-the-spatial-metric.md) gives

$$
K_{ij}K^{ij}-K^2=\frac1h\left(\pi^{ij}\pi_{ij}-\frac12\pi^2\right).
$$

To integrate the shift term without ambiguity about [tensor densities](../../../../../../tensor-density.md), put $p^{ij}=\pi^{ij}/\sqrt h$. Metric compatibility of the [spatial covariant derivative](../../../../../../spatial-covariant-derivative.md) gives, up to a boundary term,

$$
\int d^3x\,2\sqrt h\,p^{ij}D_iN_j
=-\int d^3x\,2\sqrt h\,N^iD_jp^j{}_i.
$$

Thus the [Hamiltonian formulation of general relativity](../../../../../../hamiltonian-formulation-of-general-relativity.md) has

$$
\boxed{\begin{aligned}
H&=\int d^3x\sqrt h(N\mathcal H+N^i\mathcal H_i),\\
\mathcal H&=\frac{\pi^{ij}\pi_{ij}-\pi^2/2}{h}-{}^{(3)}R,\\
\mathcal H_i&=-2D_j\left(\frac{\pi^j{}_i}{\sqrt h}\right).
\end{aligned}}
$$

Variation of the [lapse function](../../../../../../lapse-function.md) imposes the [Hamiltonian constraint](../../../../../../hamiltonian-constraint.md) $\mathcal H=0$, while variation of the [shift vector](../../../../../../shift-vector.md) imposes the [momentum constraint](../../../../../../momentum-constraint.md) $\mathcal H_i=0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
