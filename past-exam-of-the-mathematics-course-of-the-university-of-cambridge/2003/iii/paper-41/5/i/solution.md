<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $n\geq2$, the [probability integral transform](../../../../../../probability-integral-transform.md) makes $U_i=F(X_i)$ iid uniform on $[0,1]$. Continuity of $F$ is enough; strict increase is unnecessary. Their extreme [order statistics](../../../../../../order-statistic.md) have joint density

$$
f_{U_{(1)},U_{(n)}}(u,v)=n(n-1)(v-u)^{n-2},\qquad0<u<v<1:
$$

choose the observations giving the two extremes and put the remaining $n-2$ between them. Transform to $r=v-u$ and integrate $u$ from zero to $1-r$. The [uniformized sample range](../../../../../../uniformized-sample-range.md) therefore has

$$
\boxed{f_R(r)=n(n-1)r^{n-2}(1-r),\quad F_R(r)=nr^{n-1}-(n-1)r^n,\quad0<r<1.}
$$

Equivalently $R\sim\operatorname{Beta}(n-1,2)$. For $n=1$, the range is identically zero instead.

The exact failure probability is

$$
\mathbb P(R<1-\varepsilon)=(1-\varepsilon)^{n-1}[1+(n-1)\varepsilon].
$$

Thus the exact integer sample size is the least $n\geq2$ making this quantity at most $\delta$. For $\varepsilon\downarrow0$ with $n\varepsilon\to\vartheta>0$, it tends to $(1+\vartheta)e^{-\vartheta}$. This function decreases strictly from one to zero on positive $\vartheta$, because its derivative is $-\vartheta e^{-\vartheta}$. For $0<\delta<1$ there is therefore exactly one positive solution of

$$
(1+\vartheta)e^{-\vartheta}=\delta,\qquad\text{equivalently}\quad1+\vartheta-\delta e^\vartheta=0.
$$

This gives the [extreme-order-statistic tolerance interval](../../../../../../extreme-order-statistic-tolerance-interval.md) sample-size rule

$$
\boxed{n\approx\vartheta/\varepsilon.}
$$

When $\delta$ is small, $\vartheta=\log(1/\delta)+\log(1+\vartheta)$, so a useful first refinement is $\vartheta\approx\log(1/\delta)+\log\log(1/\delta)$. This is an approximation, not an exact integer guarantee; use the preceding exact failure probability to check rounding and very stringent tail requirements. The interval here encloses population content, rather than estimating a fixed distribution parameter.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
