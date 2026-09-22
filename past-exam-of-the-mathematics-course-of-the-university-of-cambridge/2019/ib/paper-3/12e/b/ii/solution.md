<h1 id="12e/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $f,g\in X$, the Lipschitz condition gives

$$
\begin{aligned}
t^{-c}\|\phi(f)(t)-\phi(g)(t)\|
&\leq Mt^{-c}\int_1^t\|f(l)-g(l)\|\,dl\\
&\leq M\|f-g\|_c\,t^{-c}\int_1^t l^c\,dl\\
&=\frac{M}{c+1}(t-t^{-c})\|f-g\|_c\\
&\leq\frac{Mb}{c+1}\|f-g\|_c.
\end{aligned}
$$

Choose $c$ so that $c+1>Mb$. Then $\phi$ is a [contraction mapping](../../../../../../../contraction-mapping.md). The space $X$ is complete in the sup norm, and therefore also in the equivalent weighted norm.

For initial value $y_0$, define

$$
\Phi_{y_0}(f)(t)=y_0+\int_1^tF(l,f(l))\,dl.
$$

It has the same contraction constant. The [Banach fixed-point theorem](../../../../../../../contraction-mapping-theorem.md) gives a unique fixed point $f$, which satisfies the integral equation. The [fundamental theorem of calculus](../../../../../../../fundamental-theorem-of-calculus.md) then gives

$$
f'(t)=F(t,f(t)),
\qquad f(1)=y_0.
$$

Conversely every solution satisfies that integral equation, proving uniqueness on $[1,b]$. This weighted-norm argument is the [Bielecki norm method](../../../../../../../bielecki-norm-method.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [12E](../../../12e.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ib](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
