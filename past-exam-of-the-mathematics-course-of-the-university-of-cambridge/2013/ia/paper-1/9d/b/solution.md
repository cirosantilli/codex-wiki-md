<h1 id="9d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md) says that, if $f$ has $N+1$ [continuous](../../../../../../continuous-function.md) derivatives on the interval joining $0$ and $x$, then for some $\xi$ strictly between them,

$$
f(x)=\sum_{j=0}^N\frac{f^{(j)}(0)}{j!}x^j+
\frac{f^{(N+1)}(\xi)}{(N+1)!}x^{N+1}.
$$

More generally the expansion is about any base point, replacing $x$ by its displacement. The displayed regularity is a sufficient hypothesis for the theorem.

For $f(t)=(1+t)^{1/2}$ and $t>-1$, repeated differentiation gives

$$
f^{(n)}(t)=\left[\frac12\left(\frac12-1\right)\cdots\left(\frac12-n+1\right)\right](1+t)^{1/2-n}.
$$

Therefore the requested coefficients are $c_n=f^{(n)}(0)/n!$. For a fixed $0<x<1$, the remainder has

$$
|R_N(x)|=|c_{N+1}|(1+\xi)^{-N-1/2}x^{N+1}\leq |c_{N+1}|x^{N+1},\qquad0<\xi<x.
$$

Now $|c_1|=1/2$ and $|c_{n+1}/c_n|=(n-1/2)/(n+1)<1$ for $n\geq1$, so $|c_{N+1}|\leq1/2$. Hence $|R_N(x)|\leq x^{N+1}/2\to0$. Passing to the limit proves, rather than merely formally suggests, the [binomial series](../../../../../../binomial-series.md)

$$
\boxed{\sqrt{1+x}=1+\sum_{n=1}^\infty c_nx^n\qquad(0<x<1).}
$$

The restriction $x>0$ makes the remainder bound especially direct, since $1+\xi\geq1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
