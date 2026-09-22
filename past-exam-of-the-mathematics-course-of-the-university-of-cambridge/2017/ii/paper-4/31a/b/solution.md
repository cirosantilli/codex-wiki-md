<h1 id="31a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $F(x)=x(\mu-x^2)$, the [fixed points](../../../../../../fixed-point.md) are zero for all $\mu$ and $\pm\sqrt{\mu-1}$ for $\mu>1$. Their multipliers are respectively $\mu$ and $3-2\mu$, giving attraction for $-1<\mu<1$ and $1<\mu<2$ respectively.

Remove these [fixed points](../../../../../../fixed-point.md) from the roots of $F^2(x)=x$. The factor $\mu+1-x^2$ gives the genuine two-cycle

$$
\boxed{\{+\sqrt{\mu+1},-\sqrt{\mu+1}\},\qquad\mu>-1.}
$$

Its multiplier is $(2\mu+3)^2>1$, so it is always unstable. It collapses to zero at $\mu=-1$, the subcritical [period-doubling bifurcation](../../../../../../period-doubling-bifurcation.md) of zero.

The remaining equation is $x^4-\mu x^2+1=0$, whose positive roots in $x^2$ exist only for $\mu\geq2$. At $\mu=2$ they give the [fixed points](../../../../../../fixed-point.md) $\pm1$, not genuine two-cycles. For $\mu>2$, put $r=\sqrt{(\mu+\sqrt{\mu^2-4})/2}>1$. Since $\mu=r^2+r^{-2}$, $F(r)=r^{-1}$ and $F(r^{-1})=r$. There are exactly two further cycles,

$$
\boxed{\{r,r^{-1}\},\qquad\{-r,-r^{-1}\},\qquad\mu>2.}
$$

Their common multiplier is $(\mu-3r^2)(\mu-3r^{-2})=9-2\mu^2$. They are attracting for $2<\mu<\sqrt5$ and repelling for $\mu>\sqrt5$, with marginal multiplier $-1$ at $\sqrt5$. Thus there are no cycles for $\mu\leq-1$, one for $-1<\mu\leq2$, and three for $\mu>2$.

<a id="31a/b/image-fixed-points-and-two-cycle-points-for-the-odd-cubic-map"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4-two-cycles.png)

**[Figure 4](#31a/b/image-fixed-points-and-two-cycle-points-for-the-odd-cubic-map). Fixed points and two-cycle points for the odd cubic map**.

The nonzero [fixed points](../../../../../../fixed-point.md) emerge in a supercritical [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) at one and each flips to an attracting two-cycle at two. Beyond $\sqrt5$ further period doubling to four-cycles is expected, followed by additional bifurcations and potentially chaotic dynamics. This local expectation does not assert chaos for every larger parameter; periodic windows and escape are possible.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31A](../../31a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
