<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [non-degenerate probability distribution](../../../../../non-degenerate-probability-distribution.md) is not concentrated at a single point. In [extreme value theory](../../../../../extreme-value-theory.md), a non-degenerate [distribution function](../../../../../cumulative-distribution-function.md) $F$ is [max-stable](../../../../../max-stable-distribution.md) if, for each integer $n\geq1$, constants $a_n>0,b_n\in\mathbb R$ satisfy $F(a_nx+b_n)^n=F(x)$ for every $x$. This says that a normalized [sample maximum](../../../../../sample-maximum.md) has the same law as one observation. A [distribution function](../../../../../cumulative-distribution-function.md) $F$ belongs to the [maximum domain of attraction](../../../../../maximum-domain-of-attraction.md) of a non-degenerate $G$ if there are $a_n>0,b_n$ such that

$$
F(a_nx+b_n)^n\longrightarrow G(x)
$$

at every [continuity](../../../../../continuous-function.md) point of $G$. Equivalently, $(M_n-b_n)/a_n$ has [convergence in distribution](../../../../../convergence-in-distribution.md) to $G$.

The [extremal types theorem](../../../../../extremal-types-theorem.md) says that any such non-degenerate limit is [max-stable](../../../../../max-stable-distribution.md) and, up to a positive affine change of variable, is exactly one of the following:

$$
\begin{aligned}
\Lambda(x)&=e^{-e^{-x}},&&x\in\mathbb R,\\
\Phi_\alpha(x)&=e^{-x^{-\alpha}},&&x>0,\quad \Phi_\alpha(x)=0\ (x\leq0),\\
\Psi_\alpha(x)&=e^{-(-x)^\alpha},&&x<0,\quad \Psi_\alpha(x)=1\ (x\geq0),
\end{aligned}
\qquad\alpha>0.
$$

These are respectively the [Gumbel distribution](../../../../../gumbel-distribution.md), [Fréchet distribution](../../../../../frechet-distribution.md), and [negative Weibull distribution](../../../../../negative-weibull-distribution.md). The theorem is also known as the [Fisher–Tippett–Gnedenko theorem](../../../../../extremal-types-theorem.md).

Useful sufficient conditions can be expressed using the [survival function](../../../../../survival-function.md) $\overline F=1-F$ and the [right endpoint of a distribution](../../../../../right-endpoint-of-a-distribution.md) $x_F$. An infinite endpoint with $\overline F(tx)/\overline F(t)\to x^{-\alpha}$ for every $x>0$ gives the [Fréchet distribution](../../../../../frechet-distribution.md) domain. A finite endpoint with $\overline F(x_F-sx)/\overline F(x_F-s)\to x^\alpha$ as $s\downarrow0$ gives the [negative Weibull distribution](../../../../../negative-weibull-distribution.md) domain. For the [Gumbel distribution](../../../../../gumbel-distribution.md), it suffices that a positive [Gumbel auxiliary function](../../../../../gumbel-auxiliary-function.md) $a(t)$ gives $\overline F(t+a(t)x)/\overline F(t)\to e^{-x}$ for every real $x$ as $t\uparrow x_F$. These are [regular variation](../../../../../regular-variation.md) and exponential tail-ratio conditions; they need no proof here.

In case (i), $\overline F_1(x)=(1-x)^2$ on $0<x<1$, so the finite-endpoint ratio is exactly $x^2$. Therefore **the domain is negative Weibull with shape $2$**. With $a_n=n^{-1/2}$ and $b_n=1$,

$$
\mathbb P\{\sqrt n(M_n-1)\leq x\}
=\left(1-\frac{x^2}{n}\right)^n\longrightarrow e^{-x^2}\quad(x<0),
$$

and the limit is one for $x\geq0$.

In case (ii), $\overline F_2(t)=e^{-\lambda t}$ has exponential tail ratio with the constant [Gumbel auxiliary function](../../../../../gumbel-auxiliary-function.md) $1/\lambda$. Therefore **the domain is Gumbel**. Choosing $a_n=1/\lambda$ and $b_n=\log n/\lambda$ gives

$$
\mathbb P\{\lambda M_n-\log n\leq x\}
=\left(1-\frac{e^{-x}}n\right)^n\longrightarrow e^{-e^{-x}}.
$$

In case (iii), $\overline F_3(t)=(1+t)^{-\lambda}$ has [regular variation](../../../../../regular-variation.md) of index $-\lambda$, so **the domain is Fréchet with shape $\lambda$**. The convenient choices $a_n=n^{1/\lambda}$ and $b_n=-1$ give

$$
\mathbb P\{(M_n+1)/n^{1/\lambda}\leq x\}
=\left(1-\frac{x^{-\lambda}}n\right)^n\longrightarrow e^{-x^{-\lambda}}\quad(x>0),
$$

with limit zero for $x\leq0$.

Finally, define the [empirical distribution function](../../../../../empirical-distribution-function.md) $F_n(x)=n^{-1}\sum_{i=1}^n\mathbf1_{\{X_i\leq x\}}$. On a sample with positive threshold $t=X_{(n-k)}$ and exactly $k$ observations strictly above $t$, its [survival function](../../../../../survival-function.md) has $1-F_n(t)=k/n$. Using the [Tonelli theorem](../../../../../tonelli-theorem.md) to integrate the finite nonnegative sum gives

$$
\int_t^\infty\frac{1-F_n(x)}{1-F_n(t)}\frac{dx}{x}
=\frac1k\sum_{i:X_i>t}\int_t^{X_i}\frac{dx}{x}
=\boxed{\frac1k\sum_{j=1}^k\log\frac{X_{(n-j+1)}}{X_{(n-k)}}=\widehat\gamma_H.}
$$

This is the [Hill estimator](../../../../../hill-estimator.md) as an empirical plug-in version of the tail-integral limit. It does not prove consistency for fixed $k$; that is a separate issue.

There is a finite-sample qualification because the question permits ties and does not assume positive observations. The formula requires $1\leq k<n$ and $t>0$. If $r=\#\{i:X_i>t\}<k$ because the threshold is tied, direct substitution gives

$$
\frac1r\sum_{j=1}^k\log\frac{X_{(n-j+1)}}t\qquad(r>0),
$$

where terms equal to the threshold contribute zero. This is generally $k/r$ times the displayed [Hill estimator](../../../../../hill-estimator.md), rather than the same estimator. If $r=0$, the empirical plug-in denominator is zero. For a [continuous probability distribution](../../../../../continuous-probability-distribution-split.md) the no-tie condition holds almost surely; for a [Fréchet distribution](../../../../../frechet-distribution.md) domain and fixed $k$, the threshold is positive with probability tending to one. Thus **the stated plug-in identity holds at a positive untied threshold**, and the literal claim for all samples from an arbitrary [distribution function](../../../../../cumulative-distribution-function.md) needs this qualification.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
