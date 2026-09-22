<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The degree-$n$ [Bernstein basis](../../../../../bernstein-basis.md) is

$$
\boxed{b_i^n(t)=\binom ni t^i(1-t)^{n-i},\qquad 0\leq i\leq n.}
$$

For $0\leq t\leq1$, every basis function is nonnegative, and the [binomial theorem](../../../../../binomial-theorem.md) gives

$$
\sum_{i=0}^n b_i^n(t)=[t+(1-t)]^n=1.
$$

Therefore $P(t)=\sum_iP_i b_i^n(t)$ is a [convex combination](../../../../../convex-combination.md) of its [control points](../../../../../control-point.md). By the definition of their [convex hull](../../../../../convex-hull.md),

$$
\boxed{P([0,1])\subseteq\operatorname{conv}\{P_0,\ldots,P_n\}.}
$$

This includes the endpoints because $P(0)=P_0$ and $P(1)=P_n$. It depends on the specified parameter interval: outside it the weights need not be nonnegative.

For $n\geq1$, differentiating the basis and using the elementary binomial identities gives

$$
\frac{d}{dt}b_i^n(t)=n[b_{i-1}^{n-1}(t)-b_i^{n-1}(t)],
$$

where out-of-range basis indices are zero. Thus

$$
\begin{aligned}
P'(t)&=n\sum_{i=0}^nP_i[b_{i-1}^{n-1}(t)-b_i^{n-1}(t)]\\
&=n\sum_{i=0}^{n-1}(P_{i+1}-P_i)b_i^{n-1}(t).
\end{aligned}
$$

Hence the [Bézier derivative control polygon](../../../../../bezier-derivative-control-polygon.md) has points $n(P_{i+1}-P_i)$, and

$$
\boxed{P'(t)=\sum_{i=0}^{n-1}n\,\Delta P_i\,b_i^{n-1}(t).}
$$

In particular the endpoint [tangent vectors](../../../../../tangent-vector.md) are $n(P_1-P_0)$ and $n(P_n-P_{n-1})$. For $n=0$ the curve is constant and its [derivative](../../../../../derivative.md) is zero.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
