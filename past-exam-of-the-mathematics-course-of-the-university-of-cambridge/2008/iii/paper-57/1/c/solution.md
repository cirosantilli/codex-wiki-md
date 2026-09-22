<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The state in part (b) is symmetric in the receiving [qubits](../../../../../../qubit.md). Single out Bob using the [Dicke state](../../../../../../dicke-state.md) recursion. For $k\geq1$, the two [vectors](../../../../../../vector.md) are

$$
\begin{aligned}
|D_k^N\rangle&=\sqrt{\frac{k+1}{N}}|0\rangle|D_k^{N-1}\rangle+\sqrt{\frac{k}{N}}|1\rangle|D_{k-1}^{N-1}\rangle,\\
|D_{k+1}^N\rangle&=\sqrt{\frac{k}{N}}|0\rangle|D_{k+1}^{N-1}\rangle+\sqrt{\frac{k+1}{N}}|1\rangle|D_k^{N-1}\rangle.
\end{aligned}
$$

Distinct excitation counts give [orthogonal](../../../../../../orthogonal-vectors.md) states of the other recipients. Taking their [partial trace](../../../../../../partial-trace.md), the only surviving off-diagonal term comes from the common rest [vector](../../../../../../vector.md) $|D_k^{N-1}\rangle$. The [one-qubit reduction of Dicke-state superpositions](../../../../../../one-qubit-reduction-of-dicke-state-superpositions.md) is consequently

$$
\boxed{\rho=\frac1N\begin{pmatrix}k+|\alpha|^2&(k+1)\alpha\beta^*\\(k+1)\alpha^*\beta&k+|\beta|^2\end{pmatrix},\qquad k=\frac{N-1}{2}.}
$$

Put $p=|\alpha|^2$ and $q=|\beta|^2$, so $p+q=1$. The overlap with the input is

$$
\begin{aligned}
\langle\psi|\rho|\psi\rangle&=\frac{p(k+p)+q(k+q)+2(k+1)pq}{N}\\
&=\frac{k+p^2+q^2+2(k+1)pq}{N}=\frac{k+1+2kpq}{N}\\
&=\boxed{\frac{N+1+2|\alpha|^2|\beta|^2(N-1)}{2N}}.
\end{aligned}
$$

For $N=1$ there is no system to trace out, and the same [matrix](../../../../../../matrix.md) is $|\psi\rangle\langle\psi|$, with overlap one. For every $N>1$ the overlap is below one, even at its maximum $p=q=1/2$, so these are imperfect copies.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
