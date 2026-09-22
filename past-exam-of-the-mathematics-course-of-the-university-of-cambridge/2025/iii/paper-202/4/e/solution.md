<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $T_n=T\wedge n$, [Itô formula](../../../../../../ito-s-lemma.md) and the differential equation show that

$$
d\bigl(e^{-\lambda s}V(X_s)\bigr)
=e^{-\lambda s}\sigma(X_s)V'(X_s)dW_s
$$

up to $T$. After localization this is a martingale, and boundedness of $V$ permits optional stopping. Thus, conditionally on $X_0$,

$$
V(X_0)=\mathbb E\left[e^{-\lambda T_n}V(X_{T_n})\mid X_0\right].
$$

On $\{T<\infty\}$, path continuity gives $X_T\in\{\ell,r\}$ and hence $V(X_T)=1$. On $\{T=\infty\}$, boundedness of $V$ makes $e^{-\lambda n}V(X_n)\to0$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore yields

$$
V(X_0)=\mathbb E[e^{-\lambda T}\mid X_0]
$$

on $\{\ell<X_0<r\}$, with the stated convention when $T=\infty$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
