<h1 id="14c/solution">Solution</h1>

↑ **Parent:** [14C](../14c.md)

This is a [birth-death process](../../../../../birth-death-process.md) with birth and death rates

$$
b_n=\gamma+\beta n,
\qquad
d_n=\alpha n(n-1).
$$

Its transition diagram has the two arrows

$$
n\xrightarrow{\ \gamma+\beta n\ }n+1,
\qquad
n\xrightarrow{\ \alpha n(n-1)\ }n-1.
$$

The gain into state $n$ comes from a death in state $n+1$ or a birth in state $n-1$, while the loss is the sum of both rates out of state $n$. The [birth-death master equation](../../../../../birth-death-master-equation.md) is consequently

$$
\frac{\partial P(n,t)}{\partial t}
=\alpha n(n+1)P(n+1,t)
-[\alpha n(n-1)+\gamma+\beta n]P(n,t)
+[\gamma+\beta(n-1)]P(n-1,t).
$$

Multiplying by $n$, summing over the nonnegative integers, and shifting the summation indices shows that each birth contributes $+1$ and each death contributes $-1$. Thus the [first-moment equation of a birth-death process](../../../../../first-moment-equation-of-a-birth-death-process.md) gives

$$
\begin{aligned}
\frac{d\langle n\rangle}{dt}
&=\langle b_n-d_n\rangle\\
&=-\alpha\langle n^2\rangle
 +(\alpha+\beta)\langle n\rangle+\gamma.
\end{aligned}
$$

At a stationary state, use the [variance](../../../../../variance-split.md) identity $\langle n^2\rangle=\langle n\rangle^2+(\Delta n)^2$. Solving the resulting [quadratic equation](../../../../../quadratic-equation.md) gives

$$
\langle n\rangle
=\frac{\alpha+\beta}{2\alpha}
\mathbin{\pm}
\sqrt{\frac{(\alpha+\beta)^2}{4\alpha^2}
 +\frac\gamma\alpha-(\Delta n)^2}.
$$

The minus root is inadmissible whenever it is negative, namely when $(\Delta n)^2<\gamma/\alpha$. Equality would give zero mean, which is also incompatible with a positive immigration rate $\gamma$, so for $\gamma>0$ the minus branch requires $(\Delta n)^2>\gamma/\alpha$ even to be a possible mean.

For a continuum approximation, write $b(n)=\gamma+\beta n$ and $d(n)=\alpha n(n-1)$. Applying the [Kramers-Moyal expansion](../../../../../kramers-moyal-expansion.md) to the two gain terms and retaining derivatives through second order gives the [Fokker-Planck equation](../../../../../fokker-planck-equation.md)

$$
\frac{\partial P}{\partial t}
=\frac{\partial}{\partial n}[g(n)P]
 +\frac12\frac{\partial^2}{\partial n^2}[h(n)P],
$$

where the negative drift and infinitesimal jump variance are

$$
\begin{aligned}
g(n)&=d(n)-b(n)
=\alpha n^2-(\alpha+\beta)n-\gamma,\\
h(n)&=d(n)+b(n)
=\alpha n^2+(\beta-\alpha)n+\gamma.
\end{aligned}
$$

This truncation requires the typical population and the scale on which $P$ varies to be much larger than the unit jump size, with the rates varying smoothly across that scale.

The positive zero of $g$ is

$$
n_*
=\frac{\alpha+\beta+sqrt{(\alpha+\beta)^2+4\alpha\gamma}}{2\alpha}
=\frac\beta\alpha+1+\frac\gamma\beta+O(\alpha),
$$

so in particular $n_*\sim\beta/\alpha$ as $\alpha/\beta\to0$. Put $x=n-n_*$. The [linear noise approximation](../../../../../linear-noise-approximation.md) uses

$$
g(n)=g_*'x+O(x^2),
\qquad h(n)=h_*+O(x),
$$

where

$$
g_*'=2\alpha n_*-(\alpha+\beta)
=\sqrt{(\alpha+\beta)^2+4\alpha\gamma}>0
$$

and, because $b(n_*)=d(n_*)$,

$$
h_*=h(n_*)=2b(n_*)=2(\gamma+\beta n_*).
$$

In a stationary state with zero [Fokker-Planck probability current](../../../../../fokker-planck-probability-current.md),

$$
g_*'xP+\frac{h_*}{2}\frac{dP}{dx}=0.
$$

Its normalized solution is the [normal distribution](../../../../../normal-distribution.md)

$$
P(x)\simeq
\sqrt{\frac{g_*'}{\pi h_*}}
\exp\left(-\frac{g_*'x^2}{h_*}\right).
$$

It follows that

$$
\langle n\rangle\simeq n_*\sim\frac\beta\alpha,
\qquad
(\Delta n)^2\simeq\frac{h_*}{2g_*'}
\sim\frac\beta\alpha.
$$

These estimates agree with the exact stationary first-moment relation on its plus branch to leading order: inserting $(\Delta n)^2\sim\beta/\alpha$ gives $\langle n\rangle\sim\beta/\alpha$. Moreover,

$$
\frac{\Delta n}{n_*}sim\sqrt{\frac\alpha\beta}\ll1,
\qquad
\Delta n\sim\sqrt{\frac\beta\alpha}\gg1.
$$

**Thus the stationary mass lies far from the boundary $n=0$, is narrow relative to its mean, yet changes across many lattice sites. These are precisely the large-population and slow-variation conditions needed for the diffusion approximation.**

## ↑ Ancestors (10)

1. [14C](../14c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
