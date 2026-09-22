<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A shift-invariant basis is a common [eigenbasis](../../../../../../eigenbasis.md) of all [cyclic shift operators](../../../../../../cyclic-shift-operator.md) $U(\gamma)$. For the displayed Fourier states, [orthonormality](../../../../../../orthonormal-set.md) follows from the [root-of-unity filter](../../../../../../root-of-unity-filter.md):

$$
\langle\xi_\alpha|\xi_{\alpha'}\rangle
=\frac1N\sum_{\beta\in\mathbb Z_N}
\omega^{(\alpha-\alpha')\beta}
=\delta_{\alpha,\alpha'}.
$$

There are $N$ vectors in this [orthonormal set](../../../../../../orthonormal-set.md) in the $N$-dimensional [Hilbert space](../../../../../../hilbert-space-split.md), so they form a [basis](../../../../../../basis.md). Reindexing the finite sum gives

$$
\begin{aligned}
U(\gamma)|\xi_\alpha\rangle
&=\frac1{\sqrt N}\sum_\beta
\omega^{-\alpha\beta}|\beta+\gamma\rangle\\
&=\omega^{\alpha\gamma}|\xi_\alpha\rangle.
\end{aligned}
$$

**Thus every $|\xi_\alpha\rangle$ is simultaneously an [eigenvector](../../../../../../eigenvector.md) of every shift, with [eigenvalue](../../../../../../eigenvalue.md) $\omega^{\alpha\gamma}$ for $U(\gamma)$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
