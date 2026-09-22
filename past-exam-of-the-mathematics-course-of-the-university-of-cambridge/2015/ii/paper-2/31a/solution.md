<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

For [spin](../../../../../spin.md) $1/2$, **$\mathbf S=\hbar\boldsymbol\sigma/2$**. The [Pauli matrices](../../../../../pauli-matrices.md) satisfy $\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k$. The antisymmetric term vanishes on contraction with $n_in_j$, and $|\mathbf n|=1$, so $(\mathbf n\cdot\boldsymbol\sigma)^2=I$. Separating the even and odd terms of the exponential series gives

$$
\boxed{e^{-i\theta\mathbf n\cdot\mathbf S/\hbar}=I\cos(\theta/2)-i(\mathbf n\cdot\boldsymbol\sigma)\sin(\theta/2).}
$$

For the single-particle [Hamiltonian](../../../../../hamiltonian.md), [unitary time evolution](../../../../../unitary-time-evolution.md) consequently acts as

$$
|\uparrow\rangle\mapsto\cos(\alpha t/2)|\uparrow\rangle-i\sin(\alpha t/2)|\downarrow\rangle,\qquad|\downarrow\rangle\mapsto\cos(\alpha t/2)|\downarrow\rangle-i\sin(\alpha t/2)|\uparrow\rangle.
$$

For two [spins](../../../../../spin.md) the joint eigenstates of total [angular momentum](../../../../../angular-momentum.md) are the [spin-one-half triplet state](../../../../../spin-one-half-triplet-state.md)

$$
|1,1\rangle=|\uparrow\uparrow\rangle,\quad |1,0\rangle=\frac{|\uparrow\downarrow\rangle+|\downarrow\uparrow\rangle}{\sqrt2},\quad |1,-1\rangle=|\downarrow\downarrow\rangle,
$$

with $J^2=2\hbar^2$ and $J_3=m\hbar$, and the [spin-one-half singlet state](../../../../../spin-one-half-singlet-state.md)

$$
|0,0\rangle=\frac{|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle}{\sqrt2},\qquad J^2=J_3=0.
$$

These follow by adding the two spin-$1/2$ angular momenta, or by direct action of the Pauli matrices.

The two terms of the specified [Hamiltonian](../../../../../hamiltonian.md) commute, so its evolution factorizes into rotations with opposite angles on the two tensor factors. The unique initial $J_3=\hbar$ state is $|\uparrow\uparrow\rangle$. With $c=\cos(\lambda t/2)$, $s=\sin(\lambda t/2)$, its evolved state is

$$
c^2|\uparrow\uparrow\rangle+s^2|\downarrow\downarrow\rangle+ics(|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle).
$$

The singlet amplitude is $i\sqrt2cs$, giving the requested probability

$$
\boxed{\mathbb P(J^2=0)=2c^2s^2=\tfrac12\sin^2(\lambda t).}
$$

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
