<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\ell(x,u)=t_+(x,u)-t_-(x,u)$ and let

$$
a(x)=\frac1{2\pi}\int_0^{2\pi}\mathbf1_{\{\ell(x,u_\theta)>0\}}\,d\theta>0.
$$

This is the accepted fraction of directions when zero-length chords are redrawn; it equals one in the interior. The [Markov kernel](../../../../../../markov-kernel.md) integrates a test function $h$ as

$$
Ph(x)=\frac1{2\pi a(x)}\int_{\ell(x,u_\theta)>0}\frac1{\ell(x,u_\theta)}
\int_{t_-}^{t_+}h(x+tu_\theta)\,dt\,d\theta.
$$

The signed polar representation has [Jacobian determinant](../../../../../../jacobian-determinant.md) $|t|$. Each point $y\ne x$ is represented twice, once with positive $t$ and once with negative $t$ and the opposite direction. Since the chord is the same in either representation, the [hit-and-run kernel density](../../../../../../hit-and-run-kernel-density.md) is

$$
\boxed{p(x,y)=\frac1{\pi a(x)\ell(x,(y-x)/|y-x|)|y-x|}\quad(y\ne x)}
$$

for almost every $y\in\mathcal C$, and it is zero outside the body. Thus the transition is absolutely continuous with respect to planar [Lebesgue measure](../../../../../../lebesgue-measure.md). Redrawing removes the only potential zero-chord atoms.

Let $D=\operatorname{diam}(\mathcal C)>0$. For distinct $x,y\in\mathcal C$, the chord contains their segment, so it has positive length, and

$$
a(x)\leq1,\qquad\ell(x,u)\leq D,\qquad |y-x|\leq D.
$$

Hence $p(x,y)\geq1/(\pi D^2)$. Values on the diagonal, and on other null sets where a density is only specified almost everywhere, can be assigned this same lower bound. This gives a version satisfying

$$
\boxed{\inf_{x,y\in\mathcal C}p(x,y)\geq\frac1{\pi D^2}>0.}
$$

For interior $x,y$, $a(x)=a(y)=1$ and the chord length is unchanged on interchanging its endpoints, so $p(x,y)=p(y,x)$. A convex body's boundary has area zero; for example contractions about an interior point fill the interior and their areas tend to the body's area. Thus this symmetry holds almost everywhere for two uniform points, proving [detailed balance](../../../../../../detailed-balance.md) and stationarity of the [uniform distribution](../../../../../../continuous-uniform-distribution.md). Without positive area or the boundary convention in part (a), the literal assertion need not hold.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
