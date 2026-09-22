# Two-dimensional triangular model of transient growth

↑ **Parent:** [Transient growth](transient-growth.md)

For $L=\begin{pmatrix}\lambda_1&0\\1&\lambda_2\end{pmatrix}$ with distinct real negative [eigenvalues](eigenvalue.md), the [matrix exponential](matrix-exponential.md) is $A=\begin{pmatrix}a&0\\b&d\end{pmatrix}$, where $a=e^{\lambda_1t}$, $d=e^{\lambda_2t}$ and $b=(a-d)/(\lambda_1-\lambda_2)$. The [optimal energy amplification of a linear system](optimal-energy-amplification-of-a-linear-system.md) is

$$
G(t)=\frac{a^2+b^2+d^2+\sqrt{(a^2+b^2+d^2)^2-4a^2d^2}}2.
$$

Its [eigenvectors](eigenvector.md) are [nonorthogonal](nonorthogonal-vectors.md), and immediate energy growth occurs exactly when $\lambda_1\lambda_2<1/4$. If $\lambda_2>\lambda_1$, putting $\alpha=(\lambda_2-\lambda_1)^{-1}$ gives $G(t)\sim(1+\alpha^2)e^{2\lambda_2t}$. The optimal asymptotic initial direction $(\alpha,1)$ is an [adjoint eigenvector](left-eigenvector.md), while the eventual state aligns with the right [eigenvector](eigenvector.md) $(0,1)$.

**Table of contents**

- [Optimal time and gain of a Reynolds-scaled triangular model](optimal-time-and-gain-of-a-reynolds-scaled-triangular-model.md)
- [Orientation interval for transient energy growth](orientation-interval-for-transient-energy-growth.md)
- [Energy-neutral rotational nonlinearity](energy-neutral-rotational-nonlinearity.md)

## ↑ Ancestors (9)

1. [Transient growth](transient-growth.md)
2. [Non-normal matrix](non-normal-matrix.md)
3. [Normal matrix](normal-matrix.md)
4. [Operator theory](linear-operator-theory-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
