<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

The [Liouville theorem](../../../../../liouville-theorem.md) states that every bounded [entire function](../../../../../entire-function.md) is constant.

By the [Laurent theorem](../../../../../laurent-theorem.md), $f$ has a unique [Laurent series](../../../../../laurent-series.md) $f(z)=\sum_{n=-\infty}^\infty c_nz^n$ on $R<|z|<S$. Split it into

$$
\boxed{g(z)=\sum_{n=0}^\infty c_nz^n,\qquad h(z)=\sum_{m=1}^\infty c_{-m}z^{-m}.}
$$

Here $g$ is [holomorphic](../../../../../holomorphic-function-split.md) on $D_S$ and $h$ is [holomorphic](../../../../../holomorphic-function-split.md) on $A_{R,\infty}$. To check their extended regions of convergence explicitly, fix $r\in(R,S)$ and put $M_r=\max_{|z|=r}|f(z)|$. The [Laurent coefficient](../../../../../laurent-coefficient.md) formula gives

$$
|c_n|\leq M_rr^{-n}\quad(n\geq0),\qquad |c_{-m}|\leq M_rr^m\quad(m\geq1).
$$

The first bound ensures convergence uniformly on every closed [disk](../../../../../disk-mathematics.md) $|z|\leq r'<r$; letting $r$ range up to $S$ covers $D_S$. The second gives convergence uniformly on $|z|\geq r''>r$; letting $r$ range down to $R$ covers $A_{R,\infty}$. Locally uniform convergence of these [power series](../../../../../power-series.md), in $z$ and $1/z$ respectively, proves the claimed [holomorphy](../../../../../holomorphic-function-split.md). On the original [annulus](../../../../../annulus-mathematics.md) their sum is $f$.

The second estimate also proves $h(z)\to0$ as $|z|\to\infty$: for any fixed $r\in(R,S)$ and $|z|>r$,

$$
|h(z)|\leq M_r\sum_{m=1}^\infty(r/|z|)^m=\frac{M_rr}{|z|-r}\longrightarrow0.
$$

For uniqueness under this condition, suppose $f=g_1+h_1=g_2+h_2$. Define $F=g_1-g_2$ on $D_S$ and $F=h_2-h_1$ on $A_{R,\infty}$. The two definitions agree on the overlap, and their [domains](../../../../../domain-mathematical-analysis.md) cover $\mathbb C$, so they define an [entire function](../../../../../entire-function.md). Moreover, $F(z)\to0$ at infinity. It is bounded outside a large [disk](../../../../../disk-mathematics.md) by this limit, and inside by [continuity](../../../../../continuous-function.md) and the [extreme value theorem](../../../../../extreme-value-theorem.md). The [Liouville theorem](../../../../../liouville-theorem.md) makes $F$ constant, and its limit makes that constant zero. Hence $g_1=g_2$ and $h_1=h_2$. Without the limiting condition, adding a constant to $g$ and subtracting it from $h$ would preserve the decomposition.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [5](../../../5.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
