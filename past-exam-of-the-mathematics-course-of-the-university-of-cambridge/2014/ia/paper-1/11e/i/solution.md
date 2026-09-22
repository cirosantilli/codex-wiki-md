<h1 id="11e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $x\ne0$, put $P(t)=\sum_{k=0}^{n-1}f^{(k)}(0)t^k/k!$ and $K=(f(x)-P(x))/x^n$. The auxiliary function $F(t)=f(t)-P(t)-Kt^n$ satisfies

$$
F(x)=F(0)=0,\qquad F^{(j)}(0)=0\quad(1\leq j\leq n-1).
$$

[Rolle's theorem](../../../../../../rolle-theorem.md) first gives a zero of $F'$ strictly between zero and $x$. Apply [Rolle's theorem](../../../../../../rolle-theorem.md) to $F'$ between that zero and zero, where $F'(0)=0$, to obtain a zero of $F''$. Continue in this way. The [derivatives](../../../../../../derivative.md) through order $n-1$ are [continuous](../../../../../../continuous-function.md), since they are differentiable; hence every application is valid even if $f^{(n)}$ is not [continuous](../../../../../../continuous-function.md). After $n$ applications there is $c$ strictly between zero and $x$ with $F^{(n)}(c)=0$.

But $F^{(n)}(c)=f^{(n)}(c)-n!K$, so $K=f^{(n)}(c)/n!$. Writing $c=\theta x$ yields **the Taylor formula with Lagrange remainder**

$$
\boxed{f(x)=\sum_{k=0}^{n-1}\frac{f^{(k)}(0)}{k!}x^k
+\frac{f^{(n)}(\theta x)}{n!}x^n,\qquad0<\theta<1.}
$$

The same construction using repeated applications of [Rolle's theorem](../../../../../../rolle-theorem.md) applies when $x<0$, with intervals ordered from $x$ to zero. For $x=0$ the identity is immediate and any $\theta\in(0,1)$ works. This proves the [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md) using only the allowed theorem and elementary differentiation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
