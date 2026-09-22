<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $U_t=(1,0,0)+(B_t^1,B_t^2,B_t^3)$, with three [independent](../../../../../../independent-random-variables.md) standard [Brownian motions](../../../../../../brownian-motion-split.md), and set $R_t=|U_t|$ and $M_t=R_t^{-1}$. The radial [stochastic process](../../../../../../stochastic-process-split.md) $R$ is a three-dimensional [Bessel process](../../../../../../bessel-process.md), which never hits zero by the [Hitting-zero classification for a Bessel process](../../../../../../hitting-zero-classification-for-a-bessel-process.md). In three dimensions $u\mapsto|u|^{-1}$ is a [harmonic function](../../../../../../harmonic-function.md) away from zero: direct differentiation gives $\Delta(|u|^{-1})=0$.

For the [stopping times](../../../../../../stopping-time.md) $T_n=\inf\{t:R_t\notin(1/n,n)\}$, $n\geq2$, the [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
M_{t\wedge T_n}=1-\sum_{j=1}^3\int_0^{t\wedge T_n}\frac{U_s^j}{R_s^3}\,dB_s^j.
$$

The coefficients are bounded by $n^2$, so each stopped [Itô integral](../../../../../../ito-integral.md) is a true [martingale](../../../../../../martingale-split.md) on every finite horizon. The [stopping times](../../../../../../stopping-time.md) form a [localizing sequence](../../../../../../localizing-sequence.md); as permitted, its divergence need not be proved here. Thus $M$ is a nonnegative [continuous local martingale](../../../../../../continuous-local-martingale.md).

To see that $M$ is not a true [martingale](../../../../../../martingale-split.md), integrate the three-dimensional [multivariate normal density](../../../../../../multivariate-normal-density.md) of $U_t$ in [spherical coordinates](../../../../../../spherical-coordinate-system.md). The angular integral yields

$$
\begin{aligned}
\mathbb EM_t
&=\frac1{\sqrt{2\pi t}}\int_0^\infty\left(e^{-(r-1)^2/(2t)}-e^{-(r+1)^2/(2t)}\right)dr\\
&=2\Phi(1/\sqrt t)-1<1=\mathbb EM_0\qquad(t>0),
\end{aligned}
$$

where $\Phi$ is the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md). Therefore **the reciprocal of a three-dimensional [Bessel process](../../../../../../bessel-process.md) is a [strict local martingale](../../../../../../strict-local-martingale.md).**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
