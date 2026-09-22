<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take an environment initially in its vacuum state $|0\rangle_E$, with $|1\rangle_E$ recording an emitted photon. In atom-environment order, put $q=\sqrt{1-p}$ and $u=\sqrt p$. A [unitary dilation of amplitude damping](../../../../../../unitary-dilation-of-amplitude-damping.md) is defined by

$$
\begin{aligned}
U|00\rangle&=|00\rangle,& U|10\rangle&=q|10\rangle+u|01\rangle,\\
U|01\rangle&=q|01\rangle-u|10\rangle,& U|11\rangle&=|11\rangle.
\end{aligned}
$$

The middle two images are orthonormal, and they are orthogonal to the two fixed images. Thus this completion really is a [unitary operator](../../../../../../unitary-operator.md). For the occupied initial environmental subspace, it leaves a ground-state atom unchanged and splits an excited-state atom into no-emission and emission alternatives with probabilities $1-p$ and $p$.

Tracing out the environment after this unitary evolution gives

$$
\Phi(\rho)=\operatorname{Tr}_E\bigl[U(\rho\otimes|0\rangle\langle0|_E)U^\dagger\bigr].
$$

The environment [matrix](../../../../../../matrix.md) elements are $\langle0|_EU|0\rangle_E=A_0$ and $\langle1|_EU|0\rangle_E=A_1$, recovering the [Kraus operators](../../../../../../kraus-operator.md) in part (a). More explicitly, the basis operators transform as

$$
\begin{aligned}
|0\rangle\langle0|&\longmapsto|0\rangle\langle0|,\\
|1\rangle\langle1|&\longmapsto(1-p)|1\rangle\langle1|+p|0\rangle\langle0|,\\
|0\rangle\langle1|&\longmapsto\sqrt{1-p}|0\rangle\langle1|,\\
|1\rangle\langle0|&\longmapsto\sqrt{1-p}|1\rangle\langle0|.
\end{aligned}
$$

Applying linearity to the atomic [density operator](../../../../../../density-matrix.md) therefore yields

$$
\boxed{\Phi(\rho)=\begin{pmatrix}
\rho_{00}+p\rho_{11}&\sqrt{1-p}\,\rho_{01}\\
\sqrt{1-p}\,\rho_{10}&(1-p)\rho_{11}
\end{pmatrix}.}
$$

The lost excited population goes to the ground state, the [trace](../../../../../../matrix-trace.md) stays one, and coherences decrease by $\sqrt{1-p}$. Discarding the distinguishable environmental photon record is precisely what turns the joint unitary evolution into a noisy atomic [quantum channel](../../../../../../quantum-channel.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
