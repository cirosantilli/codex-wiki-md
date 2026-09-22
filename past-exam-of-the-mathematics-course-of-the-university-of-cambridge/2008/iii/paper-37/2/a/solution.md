<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $r=\|y\|$ and use the ordinary Euclidean [Laplacian](../../../../../../laplacian.md) $\sum_i\partial_i^2$, so the generator of standard [Brownian motion](../../../../../../brownian-motion-split.md) is half that operator. For a radial function $f(r)$, the [Laplacian in polar coordinates](../../../../../../laplacian-in-polar-coordinates.md) is $f''(r)+(d-1)f'(r)/r$. With $f(r)=r^{2-d}$,

$$
f'(r)=(2-d)r^{1-d},\qquad f''(r)=(2-d)(1-d)r^{-d},\qquad\Delta h=0\quad(r>0).
$$

Thus $h$ is a [harmonic function](../../../../../../harmonic-function.md) on the punctured space.

We first justify that the singularity is not visited. For $0<\eta<x<R$, stop at $S=\tau_\eta\wedge\tau_R$. The [Itô formula](../../../../../../ito-s-lemma.md) makes $h(B_{t\wedge S})$ a [local martingale](../../../../../../local-martingale.md), and it is bounded on this annulus, hence a true [martingale](../../../../../../martingale-split.md). The exit time is finite almost surely: $\mathbb P(S>t)\leq\mathbb P(\|B_t\|<R)\to0$ by the Gaussian transition density. Taking the bounded terminal limit yields

$$
\mathbb P(\tau_\eta<\tau_R)\,\eta^{2-d}\leq h(\bar x)=x^{2-d}.
$$

If the origin were reached before $\tau_R$, every smaller radius would first be reached, so letting $\eta\downarrow0$ shows that event has probability zero. Taking a countable sequence $R\to\infty$ proves $\tau_0=\infty$ almost surely. Localization on increasing annuli now applies the [Itô formula](../../../../../../ito-s-lemma.md) globally and gives the [Bessel power local martingale](../../../../../../bessel-power-local-martingale.md)

$$
h(B_t)=h(\bar x)+\int_0^t\nabla h(B_s)\cdot dB_s.
$$

Stopping this [continuous local martingale](../../../../../../continuous-local-martingale.md) at any $\tau_a$, including $a=0$, preserves its local-[martingale](../../../../../../martingale-split.md) property.

For $0<a<x$, the stopped path stays at radius at least $a$, so $0<M_t\leq a^{2-d}$. The [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md) makes it a true [martingale](../../../../../../martingale-split.md). For $a=x$, Brownian radial oscillations at its starting sphere give $\tau_x=0$ almost surely and the stopped process is constant. Thus the same true-[martingale](../../../../../../martingale-split.md) conclusion holds for $0<a\leq x$.

For $a=0$, the process is a [strict local martingale](../../../../../../strict-local-martingale.md). To prove this, write $B_t=\bar x+\sqrt t\,G$ in distribution, with $G$ a standard $d$-dimensional normal vector. For every shift $v$,

$$
\mathbb E\|G+v\|^{2-d}\leq1+(2\pi)^{-d/2}\int_{\|u\|\leq1}\|u\|^{2-d}\,du=:C_d<\infty.
$$

Indeed the integrand outside the unit ball is at most one, while inside it the Gaussian density is at most $(2\pi)^{-d/2}$ and the radial integral is a constant times $\int_0^1r\,dr$. [Brownian scaling](../../../../../../brownian-scaling.md) therefore gives

$$
\mathbb E h(B_t)\leq C_dt^{-(d-2)/2}\longrightarrow0.
$$

A true [martingale](../../../../../../martingale-split.md) would have expectation $h(\bar x)>0$ at every time, which is impossible.

The printed range also permits $a>x$, and this case must not be grouped with the bounded case. Here $\tau_a<\infty$ almost surely, by the same Gaussian bound for exit from a bounded ball. Moreover,

$$
\mathbb E M_t=a^{2-d}\mathbb P(\tau_a\leq t)+\mathbb E\bigl[h(B_t)\mathbf1_{\{\tau_a>t\}}\bigr]\longrightarrow a^{2-d}<x^{2-d},
$$

since the second expectation is at most $\mathbb E h(B_t)\to0$. It too is a [strict local martingale](../../../../../../strict-local-martingale.md). The complete [stopped inverse radial power martingale classification](../../../../../../stopped-inverse-radial-power-martingale-classification.md) is therefore

$$
\boxed{M\text{ is a true martingale for }0<a\leq x;\quad M\text{ is strict local for }a=0\text{ or }a>x.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
