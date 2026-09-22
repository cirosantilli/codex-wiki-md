<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The precise external concentration result we use is [Talagrand's convex distance inequality](../../../../../../talagrand-s-convex-distance-inequality.md): for a finite product of independent standard [probability spaces](../../../../../../probability-space.md), a measurable event $B$ of positive [probability](../../../../../../probability.md), and $u\geq0$,

$$
\mathbb P(B)\,\mathbb P(d_T(X,B)\geq u)\leq e^{-u^2/4}.
$$

Our coordinates are the independent uniformly sampled points of the [triangle](../../../../../../triangle.md), so the hypothesis holds. Part (ii) therefore gives, for integers $a>b\geq0$,

$$
\mathbb P(L_n\geq a)\,\mathbb P(L_n\leq b)
\leq\exp\!\left(-\frac{(a-b)^2}{4a}\right).
$$

Indeed every configuration in the first event has at least the distance from part (ii) to the second event. If one event is empty, the displayed product bound is automatic. This is the only use of the product-space theorem; the geometric separation was proved directly in part (ii). A precise source for that theorem is Section 4.1 of [Talagrand's original product-space concentration paper](https://arxiv.org/pdf/math/9406212).

Choose an integer [median](../../../../../../median.md) $m=m_n$, so $\mathbb P(L_n\leq m)\geq1/2$ and $\mathbb P(L_n\geq m)\geq1/2$. First set $a=m+t$, $b=m$ in the product bound, and then set $a=m$, $b=m-t$. For positive integers $t$ this yields the [convex-chain median concentration](../../../../../../convex-chain-median-concentration.md) estimates

$$
\boxed{\mathbb P(L_n\geq m+t)\leq2e^{-t^2/(4(m+t))},\qquad
\mathbb P(L_n\leq m-t)\leq2e^{-t^2/(4m)}.}
$$

The lower event is empty if $m-t<1$ in our sampling model; the upper event is empty if $m+t>n$. Thus the stated bounds remain valid for all positive integers $t$. Also $m\geq1$ for $n\geq1$.

By part (i), $m\leq Cn^{1/3}$ with $C=4e$. Let $h_n=\omega(n)n^{1/6}/2$, take $t_n=\lfloor h_n\rfloor+1$, and use the deterministic interval $I_n=[m-h_n,m+h_n]$. Its length is exactly $\omega(n)n^{1/6}$. As $L_n$ and $m$ are integers, falling outside this interval implies one of the two tail events with $t=t_n$. Therefore

$$
\mathbb P(L_n\notin I_n)\leq4\exp\!\left(-\frac{t_n^2}{4(m+t_n)}\right).
$$

For positive $m,t$,

$$
\frac{t^2}{4(m+t)}\geq\frac18\min\left\{\frac{t^2}{m},t\right\}.
$$

Since $t_n\geq h_n$ and $m\leq Cn^{1/3}$, this exponent is at least

$$
\frac18\min\left\{\frac{\omega(n)^2}{4C},\frac{\omega(n)n^{1/6}}2\right\}\longrightarrow\infty.
$$

Consequently

$$
\boxed{\mathbb P\!\left(L_n\in[m_n-\tfrac12\omega(n)n^{1/6},\ m_n+\tfrac12\omega(n)n^{1/6}]\right)\longrightarrow1.}
$$

Thus $L_n$ lies [with high probability](../../../../../../with-high-probability.md) in the required interval. This proof works for every $\omega(n)\to\infty$, including growth faster than $n^{1/6}$; no extra restriction on $\omega$ is needed. The scale comes from the square root of the $O(n^{1/3})$ certificate size at the [median](../../../../../../median.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
