<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $Z_m$ be the discount level during policy year $m$, with $Z_0=1$. Under the usual assumption of independent successive annual accidents and repair costs with the same laws each year, the submitted-claim decision depends only on $Z_m$ and that year's cost. Consequently the conditional distribution of $Z_{m+1}$ depends on the past only through $Z_m$: this is the [Markov property](../../../../../markov-property.md). The [no claims discount system](../../../../../no-claims-discount-system.md) is therefore a time-homogeneous [discrete-time Markov chain](../../../../../discrete-time-markov-chain.md). Stationarity of accident probabilities alone, without this independence assumption, would not by itself establish the Markov property.

At level one a claim keeps the policyholder at one, while no submitted claim moves them to two. At level two, a submitted claim moves them to one and no claim to three. At level three, a claim moves them to two and no claim keeps them at three. Thus $p_i$ in the specified [transition matrix](../../../../../stochastic-matrix.md) is the annual probability of a submitted claim at current level $i$, not merely of an accident. A small accident paid privately counts as no claim for these transitions.

Let $b>0$ denote the undiscounted annual premium. It is not specified numerically in the source; costs can instead be measured in units of that premium, giving $b=1$. The actual premium payments at the three levels are $b$, $b(1-\alpha)$, and $b(1-\beta)$. Compare the two future paths, assuming no further accidents, to obtain the [two-year premium-loss claim threshold](../../../../../two-year-premium-loss-claim-threshold.md). From level one, a current claim leads to future levels $(1,2)$, whereas no claim leads to $(2,3)$, giving extra premium

$$
h_1=b+b(1-\alpha)-b(1-\alpha)-b(1-\beta)=b\beta.
$$

From level two the two paths are $(1,2)$ and $(3,3)$, and from level three they are $(2,3)$ and $(3,3)$. Hence

$$
\boxed{h_1=b\beta,\qquad h_2=b(2\beta-\alpha),\qquad h_3=b(\beta-\alpha).}
$$

These are all strictly positive. The PDF's discount fractions are $\alpha$ and $\beta$; the converted TeX has lost these factors in the percentages.

For a repair cost $X$ with the specified [lognormal distribution](../../../../../log-normal-distribution.md), $\log X\sim N(\mu,\sigma^2)$. Put

$$
z_i=\frac{\log h_i-\mu}{\sigma},\qquad\overline\Phi(z)=1-\Phi(z),
$$

where $\Phi$ is the [standard normal distribution function](../../../../../standard-normal-distribution-function.md). Conditional on an accident, the submitted-claim probability is $\mathbb P(X>h_i)=\overline\Phi(z_i)$. Multiplying by the accident probability gives

$$
\boxed{\begin{aligned}
p_1&=p\left[1-\Phi\left(\frac{\log(b\beta)-\mu}{\sigma}\right)\right],\\
p_2&=p\left[1-\Phi\left(\frac{\log(b(2\beta-\alpha))-\mu}{\sigma}\right)\right],\\
p_3&=p\left[1-\Phi\left(\frac{\log(b(\beta-\alpha))-\mu}{\sigma}\right)\right].
\end{aligned}}
$$

Set $b=1$ for the premium-unit convention. Without a monetary premium scale, discount percentages alone cannot determine a numerical threshold for a monetary repair cost.

This nearest-neighbour [Markov chain](../../../../../markov-chain.md) is a finite [birth-death chain](../../../../../birth-death-chain.md). Its [stationary distribution](../../../../../stationary-distribution.md) $\pi$ satisfies the endpoint balance equations

$$
\pi_1(1-p_1)=\pi_2p_2,\qquad
\pi_2(1-p_2)=\pi_3p_3.
$$

These [detailed balance](../../../../../detailed-balance.md) equations also imply the middle-state balance equation. The [three-level no claims discount equilibrium](../../../../../three-level-no-claims-discount-equilibrium.md) is therefore

$$
\boxed{(\pi_1,\pi_2,\pi_3)=\frac1D\bigl(p_2p_3,\ (1-p_1)p_3,\ (1-p_1)(1-p_2)\bigr),}
$$

where

$$
D=p_2p_3+(1-p_1)p_3+(1-p_1)(1-p_2).
$$

Since each $p_i$ lies strictly between zero and one, this is an [irreducible Markov chain](../../../../../irreducible-markov-chain.md). Positive holding probabilities at the endpoints also make it an [aperiodic Markov chain](../../../../../aperiodic-markov-chain.md). Its unique [stationary distribution](../../../../../stationary-distribution.md) is the limiting distribution even from the initial level one, and gives the steady-state proportions for a homogeneous population of such policyholders.

A submitted claim at level one conditions the repair cost on $X>h_1$. The accident probability cancels in this [conditional expectation](../../../../../conditional-expectation.md). For $z_1=(\log h_1-\mu)/\sigma$, the [truncated lognormal moment](../../../../../truncated-lognormal-moment.md) follows by completing the square:

$$
\begin{aligned}
\mathbb E[X\,1_{\{X>h_1\}}]
&=\int_{z_1}^{\infty}e^{\mu+\sigma z}\frac{e^{-z^2/2}}{\sqrt{2\pi}}\,dz\\
&=e^{\mu+\sigma^2/2}\int_{z_1}^{\infty}\frac{e^{-(z-\sigma)^2/2}}{\sqrt{2\pi}}\,dz\\
&=e^{\mu+\sigma^2/2}\overline\Phi(z_1-\sigma).
\end{aligned}
$$

Dividing by $\mathbb P(X>h_1)=\overline\Phi(z_1)$ yields the expected size of an actual submitted claim:

$$
\boxed{\mathbb E[X\mid\text{claim at level one}]
=e^{\mu+\sigma^2/2}\frac{1-\Phi((\log(b\beta)-\mu-\sigma^2)/\sigma)}{1-\Phi((\log(b\beta)-\mu)/\sigma)}.}
$$

The unconditional expected amount paid per year from level one would instead multiply its tail first moment by $p$; it is not the conditional claim size requested here.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
