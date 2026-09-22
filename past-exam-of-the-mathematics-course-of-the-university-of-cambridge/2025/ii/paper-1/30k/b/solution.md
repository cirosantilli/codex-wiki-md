<h1 id="30k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $D=b^TV^{-1}b$ and decompose any $\theta$ in the $V$-inner product as

$$
\theta=\lambda\theta_M+\eta,\qquad \eta^TV\theta_M=\eta^Tb=0.
$$

Then

$$
\mathbb EX=\lambda D,\qquad
\operatorname{Var}(X)=\lambda^2D+\eta^TV\eta.
$$

For fixed $\lambda$, a nonzero $\eta$ leaves the mean unchanged and strictly raises variance, so strict monotonicity of $F$ excludes it from a maximizer. If $D>0$ and $\lambda<0$, the zero portfolio has a larger mean and smaller variance, so this is also impossible. Hence every maximizer is

$$
\theta^*=\lambda\theta_M\qquad(\lambda\geq0).
$$

If $b=0$, the unique variance-minimizing maximizer is $\theta^*=0$, which is the same conclusion with $\lambda=0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
