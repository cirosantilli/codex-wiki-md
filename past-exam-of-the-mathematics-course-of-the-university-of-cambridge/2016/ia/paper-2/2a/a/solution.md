<h1 id="2a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start from $I_0(\lambda)=1/\lambda$. [Differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) gives

$$
I_n'(\lambda)=-I_{n+1}(\lambda),\qquad I_n(\lambda)=(-1)^n\frac{d^n}{d\lambda^n}\frac1\lambda.
$$

This interchange is justified locally around any $\lambda>0$ by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md): the differentiated integrands are bounded by an integrable [polynomial](../../../../../../polynomial-split.md) times $e^{-\lambda x/2}$. Successive [derivatives](../../../../../../derivative.md) of $\lambda^{-1}$ give

$$
\boxed{I_n(\lambda)=\frac{n!}{\lambda^{n+1}}.}
$$

This is also the integer case of the [Gamma function](../../../../../../gamma-function.md) integral after scaling the integration variable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2A](../../2a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
