<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

The remaining cyclic [commutators](../../../../../commutator.md) are $[S_y,S_z]=i\hbar S_x$ and $[S_z,S_x]=i\hbar S_y$. In a spin-$s$ irreducible representation,

$$
\boxed{S_z=\hbar m_s,\quad m_s=-s,-s+1,\ldots,s;\qquad S^2=\hbar^2s(s+1)}.
$$

For [spin](../../../../../spin.md) one-half, $S_i=\hbar\sigma_i/2$, appropriate to an [electron](../../../../../electron.md)'s [spin](../../../../../spin.md). Each $S_i^2=\hbar^2I/4$, so this [Hamiltonian](../../../../../hamiltonian.md) is $H=A\hbar^2I/4$. The orthonormal vectors $(1,0)^T$ and $(0,1)^T$ are eigenstates with the same [energy](../../../../../energy-split.md) **$A\hbar^2/4$**; every normalized [superposition](../../../../../superposition-principle.md) is also an eigenstate. The $B$ term vanishes identically because [spin-one-half quadratic anisotropy is constant](../../../../../spin-one-half-quadratic-anisotropy-is-constant.md).

For the supplied three-dimensional basis one consistent choice is

$$
S_y=i\hbar\begin{pmatrix}0&0&1\\0&0&0\\-1&0&0\end{pmatrix},\qquad
S_z=i\hbar\begin{pmatrix}0&1&0\\-1&0&0\\0&0&0\end{pmatrix}.
$$

These [Hermitian matrices](../../../../../hermitian-operator.md) obey the cyclic [commutators](../../../../../commutator.md) with the given $S_x$, and $S^2=2\hbar^2I$, representing [spin](../../../../../spin.md) one. Their squares give

$$
H=\hbar^2\operatorname{diag}(A-B,A+B,0).
$$

Thus the three normalized Cartesian basis vectors $e_1,e_2,e_3$ have energies **$\hbar^2(A-B)$, $\hbar^2(A+B)$ and $0$**, respectively; degeneracies permit arbitrary orthonormal choices in the corresponding [eigenspaces](../../../../../eigenspace.md).

The parallel and antiparallel $S_x$ states are $|+x\rangle=(0,1,-i)^T/\sqrt2$ and $|-x\rangle=(0,1,i)^T/\sqrt2$. Evolution from the first gives

$$
|\psi(t)\rangle=\frac1{\sqrt2}\begin{pmatrix}0\\e^{-i(A+B)\hbar t}\\-i\end{pmatrix},\qquad
P_{-x}(t)=\sin^2\left(\frac{(A+B)\hbar t}{2}\right).
$$

This [spin-one reversal under quadratic anisotropy](../../../../../spin-one-reversal-under-quadratic-anisotropy.md) is complete when

$$
\boxed{t=\frac{(2j+1)\pi}{|A+B|\hbar},\quad j=0,1,\ldots}
$$

provided $A+B\ne0$. If $A+B=0$, its initial state is stationary up to phase and complete reversal never occurs. Assume real $A,B$ for a Hermitian [Hamiltonian](../../../../../hamiltonian.md).

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
