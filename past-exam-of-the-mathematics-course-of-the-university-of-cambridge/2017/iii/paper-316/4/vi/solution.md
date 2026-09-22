<h1 id="4/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Write $x=1/a$ for the [comet](../../../../../../comet.md)'s inverse [semi-major axis](../../../../../../semi-major-axis.md). Its [specific orbital energy](../../../../../../specific-orbital-energy.md) is $-GM_\star x/2$, so escape corresponds to $x=0$. The printed quantity

$$
s_x=\frac{10}{a_p}\frac{M_p}{M_\star}
$$

has dimensions of inverse length. It cannot, literally, be a standard variance-per-time [diffusion coefficient](../../../../../../diffusion-coefficient.md). Interpret it as the characteristic [root mean square](../../../../../../root-mean-square.md) step in $x$ per periapsis passage, as in a discrete [comet energy diffusion](../../../../../../comet-energy-diffusion.md) model.

If successive kicks are unbiased and uncorrelated, after $N$ passages the [root mean square](../../../../../../root-mean-square.md) displacement is $s_x\sqrt N$. Starting at $a_0$ gives $x_0=1/a_0$, hence $N_{\rm ej}\sim(x_0/s_x)^2$. Taking the characteristic interval to be the initial [orbital period](../../../../../../orbital-period.md) $P(a_0)$ gives

$$
\boxed{t_{\rm ej}\sim\frac{P(a_0)}{100}
\left(\frac{a_p}{a_0}\right)^2
\left(\frac{M_\star}{M_p}\right)^2
=\frac{P_p}{100}\sqrt{\frac{a_p}{a_0}}
\left(\frac{M_\star}{M_p}\right)^2}.
$$

Here $P_p=2\pi\sqrt{a_p^3/(GM_\star)}$. In particular, for $a_0\sim a_p$ this is $P_p(M_\star/M_p)^2/100$. Without specifying the initial [semi-major axis](../../../../../../semi-major-axis.md) and the time per statistically independent encounter, the PDF cannot determine a unique time.

With the convention $\langle(\Delta x)^2\rangle=2D_xt$, the actual [diffusion coefficient](../../../../../../diffusion-coefficient.md) would be $D_x=s_x^2/[2P(a_0)]$. The estimate requires $N_{\rm ej}\gg1$, [orbit](../../../../../../orbit-dynamical-system.md) crossing, and sufficient phase decorrelation. Near escape the [orbital period](../../../../../../orbital-period.md) grows, and resonant or secular correlations invalidate the simple constant-step clock. This is a characteristic diffusion scale, not an exact mean [first-passage time](../../../../../../first-passage-time.md): even an unbiased [Brownian motion](../../../../../../brownian-motion-split.md) on an unbounded half-line has an infinite mean time to reach its absorbing endpoint.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [4](../../4.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
