<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The sum needs a stated interpretation.** The original equation leaves the second bond outside explicit parentheses, with its index then formally free. The natural [translation-invariant](../../../../translation-invariance.md), equal-bond interpretation used here is the [energy](../../../../energy-split.md) $-J\sum_j\tau_j(\sigma_j+\sigma_{j+1})$. The subsequently mentioned $h$ has no term in that [energy](../../../../energy-split.md), so no [magnetic field](../../../../magnetic-field-split.md) or [single-ion anisotropy](../../../../single-ion-anisotropy.md) is added. Such an extra term would define another model and change the answer.

Let $K=\beta J$. Sum over each decorating [spin](../../../../spin.md) before summing over the remaining [spins](../../../../spin.md). The [decimation of an alternating mixed-spin chain](../../../../decimation-of-an-alternating-mixed-spin-chain.md) gives the effective [transfer matrix](../../../../transfer-matrix.md):

$$
V_{st}=\sum_{t_0=-1}^{1}e^{Kt_0(s+t)}=1+2\cosh[K(s+t)]
=\begin{pmatrix}1+2\cosh2K&3\\3&1+2\cosh2K\end{pmatrix}_{st}.
$$

No on-site entropy has been omitted: the term $1$ is the weight of the zero decorating [spin](../../../../spin.md). The [normalized](../../../../normalization.md) [eigenvectors](../../../../eigenvector.md) are $v_\pm=(1,\pm1)^{\mathsf T}/\sqrt2$, with [eigenvalues](../../../../eigenvalue.md)

$$
\boxed{\lambda_+=4+2\cosh2K=2+4\cosh^2K,\qquad \lambda_-=2\cosh2K-2=4\sinh^2K.}
$$

There are $L$ transfer steps but $2L$ physical sites, so

$$
\boxed{Z_L=\lambda_+^L+\lambda_-^L,\qquad
f=\lim_{L\to\infty}\frac{-k_BT\log Z_L}{2L}=-\frac{k_BT}{2}\log(4+2\cosh2\beta J).}
$$

The [free energy](../../../../thermodynamic-free-energy.md) per two-site [unit cell](../../../../unit-cell.md) is twice this value. At $J=0$, the formula gives $Z_L=6^L$, as required by two states on one sublattice and three on the other. As $T\to0$, the [free energy](../../../../thermodynamic-free-energy.md) per physical site tends to $-J$, the [energy](../../../../energy-split.md) of an aligned chain with two satisfied bonds per [unit cell](../../../../unit-cell.md). These checks also fix the factor of two in the site count.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
