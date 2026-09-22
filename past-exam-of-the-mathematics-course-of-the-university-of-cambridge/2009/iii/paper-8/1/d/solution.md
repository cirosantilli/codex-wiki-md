<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On the [Hardy space of the circle](../../../../../../hardy-space-of-the-circle.md) $H^2(\mathbb T)\subset L^2(\mathbb T)$, let $P_+$ be the projection onto nonnegative Fourier modes and $T_f=P_+M_f|_{H^2}$. The [Toeplitz index theorem for continuous symbols](../../../../../../toeplitz-index-theorem-for-continuous-symbols.md) states: for continuous $f$, $T_f$ is [Fredholm](../../../../../../fredholm-operator.md) exactly when $f$ never vanishes, and then

$$
\boxed{\operatorname{ind}T_f=-\operatorname{wind}(f,0),}
$$

with counterclockwise winding positive.

First, $T_fT_g-T_{fg}=-P_+M_f(I-P_+)M_gP_+$ is compact. For Laurent-polynomial symbols the negative-mode crossing involves only finitely many modes and is finite rank. Uniform approximation and $\|T_f\|\leq\|f\|_\infty$ extend this to continuous symbols. If $f$ is nonvanishing, $T_{1/f}$ is therefore a two-sided parametrix, and part (b) gives the [Fredholm](../../../../../../fredholm-operator.md) property.

Writing $n=\operatorname{wind}(f,0)$, a continuous argument along the parametrized circle increases by $2\pi n$. Removing this increase gives a periodic continuous logarithm $h$ of $z^{-n}f(z)$, so $f=z^ne^h$. The symbols $z^ne^{th}$ give a continuous [Fredholm](../../../../../../fredholm-operator.md) path from $z^n$ to $f$. Part (c) makes their indices equal. For $n\geq0$, $T_{z^n}$ is the $n$th unilateral shift, with zero kernel and $n$-dimensional cokernel. For negative $n$ it is the corresponding backward shift, with kernel dimension $-n$ and zero cokernel. In both cases the index is $-n$.

For necessity, if $f(\zeta)=0$ use the normalized Hardy kernels

$$
k_{r,\zeta}(z)=\frac{\sqrt{1-r^2}}{1-r\overline\zeta z},\qquad r\uparrow1.
$$

They have norm one and converge weakly to zero, as their inner products with each Fourier basis vector tend to zero. Their squared moduli are Poisson kernels concentrating at $\zeta$, so continuity gives $\|fk_{r,\zeta}\|_2\to0$ and hence $\|T_fk_{r,\zeta}\|_2\to0$. A [Fredholm](../../../../../../fredholm-operator.md) parametrix would imply $k_{r,\zeta}=BT_fk_{r,\zeta}+Kk_{r,\zeta}\to0$ in norm, because a [compact operator](../../../../../../compact-operator-split.md) takes this weakly null bounded family to zero in norm. This contradicts unit norm, proving the converse.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
