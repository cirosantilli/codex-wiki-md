<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose a proposal [probability density function](../../../../../probability-density-function.md) $g$ and a finite envelope constant $M$ such that $f(y)\le Mg(y)$ wherever the target has positive density. A [rejection sampling](../../../../../rejection-sampling.md) trial draws $Y\sim g$ and, independently, $U\sim\operatorname{Uniform}(0,1)$; accept $Y$ when

$$
U\le\frac{f(Y)}{Mg(Y)},
$$

otherwise repeat with fresh independent draws. For any measurable set $D$,

$$
\mathbb P(Y\in D,\mathrm{accept})
=\int_D g(y)\frac{f(y)}{Mg(y)}\,dy
=\frac1M\int_Df(y)\,dy.
$$

In particular $\mathbb P(\mathrm{accept})=1/M$, so the conditional accepted density is $f$. More explicitly, summing over the possible first accepted trial gives

$$
\sum_{k\ge1}(1-1/M)^{k-1}\frac1M\int_Df(y)\,dy=\int_Df(y)\,dy.
$$

Thus the algorithm terminates almost surely and its output has exactly the requested law.

The envelope constant satisfies $M\ge1$ and is the expected number of proposal trials for one output, by the [geometric distribution](../../../../../geometric-distribution.md) of the waiting time. This is the quantity often called the rejection rate $M$. The actual [probability](../../../../../probability.md) of rejecting a particular proposal is $1-1/M$, and the expected number of rejections before one acceptance is $M-1$; these conventions should not be conflated.

To generate a [standard normal distribution](../../../../../standard-normal-distribution.md), first generate its absolute value, whose [half-normal distribution](../../../../../half-normal-distribution.md) density is

$$
h(y)=\sqrt{\frac2\pi}e^{-y^2/2}\mathbf1_{\{y\ge0\}}.
$$

With the given [exponential distribution](../../../../../exponential-distribution.md) proposal, the density ratio is

$$
\frac{h(y)}{g(y)}=\frac{\sqrt{2/\pi}}\lambda
\exp\left(-\frac{y^2}{2}+\lambda y\right)
=\frac{\sqrt{2/\pi}}\lambda e^{\lambda^2/2}
\exp\left(-\frac{(y-\lambda)^2}{2}\right).
$$

Its maximum is at $y=\lambda$, hence the [normal rejection sampling with an exponential envelope](../../../../../normal-rejection-sampling-with-an-exponential-envelope.md) constant is

$$
\boxed{M(\lambda)=\frac{\sqrt{2/\pi}}\lambda e^{\lambda^2/2}.}
$$

Draw $Y\sim\operatorname{Exp}(\lambda)$ and a fresh uniform $U$; accept when $U\le e^{-(Y-\lambda)^2/2}$. An accepted $Y$ has density $h$. Independently choose a sign, positive or negative with [probability](../../../../../probability.md) $1/2$, and output $Z$ with that sign and magnitude $Y$. On either half-line its density is $h(|z|)/2=(2\pi)^{-1/2}e^{-z^2/2}$, proving the normal output law.

To optimize the rejection rate, differentiate

$$
\log M(\lambda)=\tfrac12\log(2/\pi)-\log\lambda+\tfrac12\lambda^2.
$$

Its derivative is $\lambda-1/\lambda$, negative before one and positive after one; equivalently its second derivative is $1+1/\lambda^2>0$. Thus

$$
\boxed{\lambda_{\mathrm{opt}}=1,\qquad M_{\min}=\sqrt{2e/\pi},\qquad
\mathbb P(\mathrm{accept})=\sqrt{\pi/(2e)}\approx0.76017.}
$$

The rejection [probability](../../../../../probability.md) is consequently about $0.23983$.

To use only uniforms, apply [inverse transform sampling](../../../../../inverse-transform-sampling.md): for an independent $U_1\in(0,1)$,

$$
Y=-\frac1\lambda\log U_1
$$

has survival [probability](../../../../../probability.md) $\mathbb P(Y>y)=e^{-\lambda y}$ for $y\ge0$. Use a second independent uniform for acceptance, and, after acceptance, a third independent uniform to choose the sign. Repeat with fresh uniforms after any rejection. No exponential generator is then needed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
