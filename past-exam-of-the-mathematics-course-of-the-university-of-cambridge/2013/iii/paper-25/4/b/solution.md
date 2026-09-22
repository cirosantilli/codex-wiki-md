<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $f(z)=1/\cosh z$. Differentiating gives

$$
f'(z)=-f(z)\tanh z,\qquad f''(z)=f(z)(2\tanh^2z-1).
$$

Therefore the diffusion operator satisfies $\frac12f''+\tanh z\,f'=-\frac12f$. Applying the [Itô formula](../../../../../../ito-s-lemma.md) to $Y_t=e^{t/2}f(X_t)$ cancels its drift:

$$
dY_t=-Y_t\tanh X_t\,dW_t.
$$

So $Y$ is a positive [local martingale](../../../../../../local-martingale.md). On every finite interval $[0,R]$, $0<Y_t\le e^{R/2}$. The [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md) makes it a true martingale on that interval. Since $R$ is arbitrary,

$$
\boxed{Y_t=\frac{e^{t/2}}{\cosh X_t}\text{ is a positive martingale},\qquad\mathbb EY_t=\frac1{\cosh x}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
