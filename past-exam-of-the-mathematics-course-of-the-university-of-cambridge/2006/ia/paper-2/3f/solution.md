<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

A real function $\phi$ on an interval is a [convex function](../../../../../convex-function.md) if

$$
\phi(\theta a+(1-\theta)b)\le\theta\phi(a)+(1-\theta)\phi(b)
$$

for all $a,b$ in its domain and $0\le\theta\le1$. For a finite-valued [random variable](../../../../../random-variable-split.md) $X$ with values $x_j$ and probabilities $p_j$, [Jensen's inequality](../../../../../jensen-s-inequality.md) states

$$
\phi\left(\sum_jp_jx_j\right)\le\sum_jp_j\phi(x_j),
\qquad\text{equivalently }\phi(\mathbb EX)\le\mathbb E\phi(X).
$$

Apply this with equal probabilities to $a,b$ and the [convex function](../../../../../convex-function.md) $\phi(t)=t^p$ on the nonnegative axis:

$$
\left(\frac{a+b}{2}\right)^p\le\frac{a^p+b^p}{2}.
$$

Multiplying by $2^p$ proves the [sharp two-term convex power bound](../../../../../sharp-two-term-convex-power-bound.md). Conversely taking $a=b>0$ forces $2^p\le2c_p$. Thus

$$
\boxed{c_p=2^{p-1}.}
$$

For $p=1$ the inequality is equality for every pair; for $p>1$ equality occurs when $a=b$.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
