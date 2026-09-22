<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [Arnold-Liouville theorem](../../../../../../liouville-arnold-theorem.md), work on a [symplectic manifold](../../../../../../symplectic-manifold.md) of dimension $2d$. Let $F_1=H,F_2,\ldots,F_d$ be [smooth functions](../../../../../../smooth-function.md) with pairwise vanishing [Poisson brackets](../../../../../../poisson-bracket.md), and suppose

$$
dF_1\wedge\cdots\wedge dF_d\ne0
$$

on a connected component $N$ of a common level. If $N$ is compact, then **$N$ is a $d$-dimensional [torus](../../../../../../torus.md)**. Its commuting [Hamiltonian vector fields](../../../../../../hamiltonian-vector-field.md) generate translations, and the [Hamiltonian](../../../../../../hamiltonian.md) motion on it is linear in angular coordinates. Compactness ensures completeness of these restricted [vector fields](../../../../../../vector-field.md).

Moreover a neighbourhood of $N$ admits [action-angle variables](../../../../../../action-angle-variables.md) $(I_1,\ldots,I_d,\theta_1,\ldots,\theta_d)$, with each angle defined modulo $2\pi$, for which

$$
\{\theta_i,I_j\}=\delta_{ij},\qquad
\{I_i,I_j\}=\{\theta_i,\theta_j\}=0,\qquad
F_j=F_j(I_1,\ldots,I_d).
$$

One compatible [symplectic form](../../../../../../symplectic-form.md) convention is $\omega=\sum_i d\theta_i\wedge dI_i$. The equations become

$$
\boxed{\dot I_i=0,\qquad \dot\theta_i=\frac{\partial H}{\partial I_i},\qquad
\theta_i(t)=\theta_i(0)+t\frac{\partial H}{\partial I_i}(I(0)).}
$$

The resulting motion is periodic when the frequencies are commensurable and otherwise quasiperiodic on a subtorus. This is [Liouville integrability](../../../../../../integrable-hamiltonian-system.md) with $d$ independent [first integrals in involution](../../../../../../first-integrals-in-involution.md). Compactness and regularity cannot be discarded from the [torus](../../../../../../torus.md) conclusion. On a general [Poisson manifold](../../../../../../poisson-manifold.md), apply this theorem on a regular [symplectic leaf](../../../../../../symplectic-leaf.md) of dimension $2d$; the ambient dimension alone does not specify the required number of integrals.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
