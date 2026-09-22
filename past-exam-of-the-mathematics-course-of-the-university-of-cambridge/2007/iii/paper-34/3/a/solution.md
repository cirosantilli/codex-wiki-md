<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The PDF's first Pauli term contains an undefined $\rho_x$. For the stated [depolarizing channel](../../../../../../quantum-depolarizing-channel.md), use $\sigma_x\rho\sigma_x$, consistently with the other two terms. This is the minimal typographical correction needed to define the intended [Pauli channel](../../../../../../pauli-channel.md).

Write $\rho=\frac12(I+\mathbf s\cdot\boldsymbol\sigma)$ using its [Bloch vector](../../../../../../bloch-vector.md). The [Pauli matrices](../../../../../../pauli-matrices.md) satisfy $\sigma_j\sigma_k\sigma_j=\sigma_k$ for $j=k$ and $-\sigma_k$ for $j\ne k$. Thus conjugating by each nonidentity Pauli matrix leaves one Bloch component unchanged and reverses the other two. Summing the three conjugates gives

$$
\sum_{j=x,y,z}\sigma_j\rho\sigma_j=\frac12(3I-\mathbf s\cdot\boldsymbol\sigma)=2I-\rho.
$$

Substitution yields

$$
\Phi(\rho)=\left(1-\frac{4p}{3}\right)\rho+\frac{2p}{3}I,
$$

so the [Pauli-mixture parametrization of qubit depolarization](../../../../../../pauli-mixture-parametrization-of-qubit-depolarization.md), with $p$ here the total error probability, gives

$$
\boxed{q=\frac{4p}{3},\qquad\Phi(\rho)=(1-q)\rho+qI/2.}
$$

There is also a genuine range error in the printed claim. For its full $0<p<1$ assumption, $0<q<4/3$, and **$0<q<1$ holds exactly when $0<p<3/4$**. For example $p=9/10$ gives $q=6/5$; on $|0\rangle\langle0|$ the output is $\operatorname{diag}(2/5,3/5)$, with negative $z$ Bloch component. No $q\in(0,1)$ could produce this output from that input, since its component would be $1-q>0$.

The corrected channel is still completely positive in the larger range: its original Pauli probabilities are $1-p,p/3,p/3,p/3$. This is [depolarizing noise weight above one](../../../../../../depolarizing-noise-weight-above-one.md); the formula with $q>1$ is not a convex mixture with weights $1-q,q$, but it has a valid [random unitary channel](../../../../../../random-unitary-channel.md) representation. The subsequent parts can therefore be solved both in the printed $q\in(0,1)$ regime and in the actual parameter range.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
