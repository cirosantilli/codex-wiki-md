<h1 id="34b/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The degenerate $E_0=9/2$ subspace has ordered basis

$$
|3,0\rangle,\qquad |1,1\rangle.
$$

Using the ladder actions,

$$
\begin{aligned}
H'|3,0\rangle
&=A^2B^\dagger|3,0\rangle
=\sqrt6\,|1,1\rangle,\\
H'|1,1\rangle
&=A^{\dagger2}B|1,1\rangle
=\sqrt6\,|3,0\rangle.
\end{aligned}
$$

Thus [degenerate perturbation theory](../../../../../../../degenerate-perturbation-theory.md) asks us to diagonalize

$$
H'\big|_{E_0}
=\begin{pmatrix}0&\sqrt6\\\sqrt6&0\end{pmatrix}.
$$

Its normalized eigenvectors and first-order energies are

$$
\boxed{
|\psi_+\rangle
=\frac{|3,0\rangle+|1,1\rangle}{\sqrt2},
\qquad
E_+=\frac92+\sqrt6\lambda
},
$$



$$
\boxed{
|\psi_-\rangle
=\frac{|3,0\rangle-|1,1\rangle}{\sqrt2},
\qquad
E_-=\frac92-\sqrt6\lambda
}.
$$

There is no order-$\lambda$ admixture from other unperturbed levels.

In fact, $H'$ preserves $n+2m$, so this two-dimensional eigenspace of $H_0$ is invariant. Directly,

$$
H'|\psi_\pm\rangle=\pm\sqrt6|\psi_\pm\rangle,
\qquad
H_0|\psi_\pm\rangle=\frac92|\psi_\pm\rangle.
$$

Therefore

$$
\boxed{
H|\psi_\pm\rangle
=\left(\frac92\pm\sqrt6\lambda\right)|\psi_\pm\rangle
}
$$

for every real $\lambda$, with no omitted higher-order terms. This is [exact diagonalization within a degenerate subspace](../../../../../../../exact-diagonalization-within-a-degenerate-subspace.md), specifically the [resonant two-to-one oscillator coupling](../../../../../../../resonant-two-to-one-oscillator-coupling.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [34B](../../../34b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
