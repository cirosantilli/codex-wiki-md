<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Because $x^{-2}$ is [integrable](../../../../../../../lebesgue-integrable-function.md) on $[1,\infty)$, the [Dominated convergence theorem](../../../../../../../dominated-convergence-theorem.md) applied to the defining integral proves that $v$ is [continuous](../../../../../../../continuous-function.md) on $\mathbb R$.

For $\lambda>0$, the [change of variables formula](../../../../../../../change-of-variables-formula.md) $t=\lambda x$ gives

$$
v(\lambda)=-i\lambda\int_\lambda^\infty\frac{e^{-it}}{t^2}\,dt,
$$

and for $\lambda<0$ the analogous formula is obtained with $e^{it}$. On either open half-line the lower endpoint stays away from zero locally, so repeated [differentiation under the integral sign](../../../../../../../differentiation-under-the-integral-sign.md) proves smoothness. Thus

$$
\boxed{v\in C(\mathbb R)\cap C^\infty(\mathbb R\setminus\{0\})}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 327](../../../../paper-327-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
