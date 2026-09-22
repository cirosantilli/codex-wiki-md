<h1 id="4h/solution">Solution</h1>

↑ **Parent:** [4H](../4h.md)

The [argument principle](../../../../../argument-principle.md) states that if $h$ is [meromorphic](../../../../../meromorphic-function.md) on a [neighbourhood](../../../../../neighbourhood-mathematics.md) of a positively oriented simple closed [contour](../../../../../complex-integration-contour.md) and its interior, with neither zeros nor poles on the [contour](../../../../../complex-integration-contour.md), then

$$
\frac1{2\pi i}\oint_\gamma\frac{h'(z)}{h(z)}\,dz=N-P,
$$

where $N$ and $P$ count its interior zeros and poles with [multiplicity](../../../../../multiplicity-mathematics.md). This integer is also the [winding number](../../../../../winding-number.md) of $h(\gamma)$ about zero.

Fix $z_0\in U$. Injectivity prevents $f$ from being constant on a [neighbourhood](../../../../../neighbourhood-mathematics.md) of $z_0$, so its [Taylor expansion](../../../../../taylor-expansion.md) has the form

$$
f(z)-f(z_0)=(z-z_0)^m h(z),\qquad m\ge1,\quad h(z_0)\ne0.
$$

Choose a small closed disk $D\subset U$, centred at $z_0$, such that $h$ and $mh+(z-z_0)h'$ are nonzero throughout $D$. Then $f-f(z_0)$ has its sole zero at $z_0$ in $D$, of [multiplicity](../../../../../multiplicity-mathematics.md) $m$, while $f'$ has no zero in $D\setminus\{z_0\}$. On its boundary let $\delta=\min|f-f(z_0)|>0$.

Choose $0<|w|<\delta$. For every $0\le t\le1$, the [holomorphic function](../../../../../holomorphic-function.md) $f-f(z_0)-tw$ is nonzero on $\partial D$. By the [argument principle](../../../../../argument-principle.md), its number of zeros is an integer given by a [contour integral](../../../../../contour-integral.md) varying continuously with $t$, hence remains $m$. At $t=1$ none of these zeros is $z_0$, so their [derivatives](../../../../../derivative.md) are nonzero and they are [simple zeros](../../../../../simple-zero.md). Thus there are $m$ distinct points taking the value $f(z_0)+w$. Injectivity forces $m=1$, proving **$f'(z_0)\ne0$ everywhere in $U$**.

## ↑ Ancestors (10)

1. [4H](../4h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
