<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Perform the [Legendre transform in mechanics](../../../../../../../legendre-transform-in-mechanics.md), using $\dot h_{ij}=2NK_{ij}+D_iN_j+D_jN_i$. The trace contraction $\pi^{ij}K_{ij}=\sqrt h(K_{ij}K^{ij}-K^2)$ gives

$$
H=\int d^3x\left[N\sqrt h(K_{ij}K^{ij}-K^2-{}^{(3)}R)+2\pi^{ij}D_iN_j\right].
$$

To avoid differentiating a [tensor density](../../../../../../../tensor-density.md) as though it were an ordinary tensor, set $p^{ij}=\pi^{ij}/\sqrt h$. Integration by parts with the [Levi-Civita connection](../../../../../../../levi-civita-connection.md) of $h$ gives

$$
\int d^3x\sqrt h\,2p^{ij}D_iN_j=-\int d^3x\sqrt h\,2N^jD_ip^i{}_j
$$

after dropping the surface term. Also

$$
K_{ij}K^{ij}-K^2=\frac1h\left(\pi^{ij}\pi_{ij}-\frac12\pi^2\right),\qquad \pi_{ij}=h_{ik}h_{jl}\pi^{kl}.
$$

Therefore the requested [Hamiltonian](../../../../../../../hamiltonian.md) is

$$
\boxed{H=\int d^3x\sqrt h\,(N\mathcal H+N^i\mathcal H_i),\quad \mathcal H=\frac{\pi^{ij}\pi_{ij}-\pi^2/2}{h}-{}^{(3)}R,\quad \mathcal H_i=-2D_j\left(\frac{\pi^j{}_i}{\sqrt h}\right).}
$$

Varying the [lapse function](../../../../../../../lapse-function.md) and [shift vector](../../../../../../../shift-vector.md) imposes the [Hamiltonian constraint](../../../../../../../hamiltonian-constraint.md) $\mathcal H=0$ and [momentum constraint](../../../../../../../momentum-constraint.md) $\mathcal H_i=0$. The total canonical generator also contains multipliers for the vanishing lapse and shift [canonical momenta](../../../../../../../canonical-momentum.md). With an asymptotic boundary, surface terms must be restored to define the [Arnowitt-Deser-Misner energy](../../../../../../../arnowitt-deser-misner-energy.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 311](../../../../paper-311-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
