<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First fix a source convention needed for physical coordinates. The PDF's displayed definition of $\sigma_z$ omits a factor of $i$: half the [commutator](../../../../../../commutator.md) of the two Hermitian transverse matrices is anti-Hermitian and cannot supply a real Bloch coordinate. The Hermitian choice consistent with the supplied dynamical matrix is

$$
\sigma_z=\frac{[\sigma_x,\sigma_y]}{2i}
=\begin{pmatrix}-1&0\\0&1\end{pmatrix}.
$$

With this convention the three Pauli expectation values use the unit-radius normalization, unlike the orthonormal coordinates of Question 2. For example, writing $K=\begin{pmatrix}0&a\\b&0\end{pmatrix}$ with $a=1+\lambda$, $b=-\lambda$, the dissipator gives rates $-(a-b)^2/2$ for $x$, $-(a+b)^2/2$ for $y$, and population equation $\dot z=b^2-a^2-(a^2+b^2)z$. The [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) adds $2\alpha z$ to $\dot x$ and $-2\alpha x$ to $\dot z$. This independently reproduces the supplied real Bloch dynamics.

Put $q=2\lambda+1$. Since $y$ decays independently, every [steady state](../../../../../../steady-state.md) has $y_*=0$. The reduced steady-state equations are

$$
q^2x_*-4\alpha z_*=0,\qquad
4\alpha x_*+(q^2+1)z_*=-2q.
$$

Their coefficient [determinant](../../../../../../determinant.md) is

$$
D=q^2(q^2+1)+16\alpha^2.
$$

It is strictly positive unless $q=0$ and $\alpha=0$. Inverting this two-by-two system gives

$$
\boxed{x_*=-\frac{8\alpha q}{D},\qquad
z_*=-\frac{2q^3}{D}.}
$$

Thus the reduced system has a unique [steady state](../../../../../../steady-state.md) except at $\alpha=0$, $\lambda=-1/2$. At that exceptional point the equations reduce to $\dot x=0$, $\dot z=-z/2$, so every $(x,0)$ is stationary; physical coordinates restrict $-1\leq x\leq1$.

As a consistency check on positivity in the nonsingular case,

$$
1-x_*^2-z_*^2=
\frac{[16\alpha^2+q^2(q^2-1)]^2}{D^2}\geq0.
$$

The calculated state is therefore in the unit Bloch disk. The original PDF correctly labels the second steady-state expression as $z_*$; the TeX conversion's repeated $x_*$ is another transcription defect, not a second formula for $x_*$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
