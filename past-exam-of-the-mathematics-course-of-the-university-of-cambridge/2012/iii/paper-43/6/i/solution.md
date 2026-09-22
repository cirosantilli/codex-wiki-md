<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For zero drift, the reflection principle gives the known [Brownian first-passage time](../../../../../../brownian-first-passage-time.md) density

$$
h_0(t)=\frac{a}{\sqrt{2\pi t^3}}e^{-a^2/(2t)},\qquad t>0.
$$

To obtain a general drift, on a fixed finite horizon use the exponential [martingale](../../../../../../martingale-split.md) $M_t=e^{cB_t-c^2t/2}$ as change-of-measure density. The [Novikov condition](../../../../../../novikov-s-condition.md) holds for constant $c$, and the [Girsanov theorem](../../../../../../girsanov-theorem.md) says that the coordinate process $B$ has drift $c$ under the new measure. Thus the hitting law of $B$ under that measure is the law of $B+ct$ under the original measure. [Conditional expectation](../../../../../../conditional-expectation.md) of $M_T$ at a hitting time bounded by $T$ equals its stopped value, by the [martingale](../../../../../../martingale-split.md) [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md). At $H_a=t$ this value is $e^{ca-c^2t/2}$. The [drifted Brownian first-passage density](../../../../../../drifted-brownian-first-passage-density.md) is obtained by multiplying $h_0$, giving **$\boxed{h_c(t)=a e^{-(a-ct)^2/(2t)}/\sqrt{2\pi t^3}}$.**

To verify the integrated formula, put $u=(a-cT)/\sqrt T$ and $v=(-a-cT)/\sqrt T$. The identity $e^{2ac}\phi(v)=\phi(u)$ for the standard normal density gives

$$
\frac d{dT}[\overline\Phi(u)+e^{2ac}\Phi(v)]=\phi(u)\frac{a+cT+a-cT}{2T^{3/2}}=h_c(T).
$$

Both terms vanish as $T\downarrow0$, so **$\boxed{\mathbb P(H_a\leq T)=\overline\Phi((a-cT)/\sqrt T)+e^{2ac}\Phi((-a-cT)/\sqrt T)}$.** The distribution has total mass one for $c\geq0$ and mass $e^{2ac}$ for $c<0$; in the latter case the remaining probability is an atom at infinity.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
