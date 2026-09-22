<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $d_i=f(X)-f_i(X^{(i)})$. The [self-bounding function](../../../../../../self-bounding-function.md) assumptions say $0\leq d_i\leq1$ and $\sum_i d_i\leq Z$. Apply [tensorization of entropy](../../../../../../tensorization-of-entropy.md) to $e^{\lambda Z}$ and the one-coordinate entropy inequality. Since $\varphi(u)=e^u-u-1$ is convex and $\varphi(td)\leq d\varphi(t)$ for $0\leq d\leq1$, the resulting bound is

$$
\operatorname{Ent}(e^{\lambda Z})
\leq\varphi(-\lambda)\mathbb E[Ze^{\lambda Z}].
$$

Writing $\psi(\lambda)=\log\mathbb E e^{\lambda(Z-\mu)}$ and dividing by the moment-generating function reduces this to

$$
\left(\frac{\psi(\lambda)}{e^\lambda-1}\right)'
\leq\mu\left(\frac{-\lambda}{e^\lambda-1}\right)'.
$$

Both sides have finite limits at zero and $\psi(0)=\psi'(0)=0$. Integrating from zero to $\lambda$, with the direction interpreted correctly when $\lambda<0$, yields

$$
\psi(\lambda)\leq\mu(e^\lambda-\lambda-1)=\mu\varphi(\lambda),
$$

which is the required inequality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
