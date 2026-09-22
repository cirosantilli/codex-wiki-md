<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with [distribution function](../../../../../cumulative-distribution-function.md) $F$, let $M_n=\max_{1\leq i\leq n}X_i$ be the [sample maximum](../../../../../sample-maximum.md). In [extreme value theory](../../../../../extreme-value-theory.md), $F$ belongs to the [maximum domain of attraction](../../../../../maximum-domain-of-attraction.md) $D(G)$ of a nondegenerate [distribution function](../../../../../cumulative-distribution-function.md) $G$ when there exist $a_n>0$ and $b_n\in\mathbb R$ such that

$$
\boxed{\mathbb P\left(\frac{M_n-b_n}{a_n}\leq x\right)=F(a_nx+b_n)^n\longrightarrow G(x)}
$$

at every continuity point of $G$. Thus the normalized [sample maxima](../../../../../sample-maximum.md) have [convergence in distribution](../../../../../convergence-in-distribution.md) to $G$.

A positive measurable function $q$ has [regular variation](../../../../../regular-variation.md) at infinity with index $\rho$, written $q\in\mathrm{RV}_\rho$, if

$$
\boxed{\frac{q(tu)}{q(t)}\longrightarrow u^\rho\quad(t\to\infty),\qquad u>0.}
$$

The case $\rho=0$ defines a [slowly varying function](../../../../../slowly-varying-function.md); equivalently a [regularly varying function](../../../../../regular-variation.md) is $q(t)=t^\rho\ell(t)$ with $\ell$ a [slowly varying function](../../../../../slowly-varying-function.md).

Write $\overline F=1-F$ for the [survival function](../../../../../survival-function.md) and $x_F=\sup\{x:F(x)<1\}$ for the [right endpoint of a distribution](../../../../../right-endpoint-of-a-distribution.md). For $\alpha>0$, use the following standard [extreme value theory](../../../../../extreme-value-theory.md) normalization conventions:

$$
\Phi_\alpha(x)=\begin{cases}\exp(-x^{-\alpha}),&x>0,\\0,&x\leq0,\end{cases}
\qquad
\Psi_\alpha(x)=\begin{cases}\exp(-(-x)^\alpha),&x<0,\\1,&x\geq0,\end{cases}
\qquad \Lambda(x)=\exp(-e^{-x}).
$$

They are respectively the [Fréchet distribution](../../../../../frechet-distribution.md), the [negative Weibull distribution](../../../../../negative-weibull-distribution.md), and the [Gumbel distribution](../../../../../gumbel-distribution.md) for maxima. The [negative Weibull distribution](../../../../../negative-weibull-distribution.md) is supported to the left of its finite endpoint; it is not the usual positive [Weibull distribution](../../../../../weibull-distribution.md).

The necessary and sufficient [maximum domain of attraction](../../../../../maximum-domain-of-attraction.md) criteria are:

- For the [Fréchet distribution](../../../../../frechet-distribution.md),$$
  \boxed{F\in D(\Phi_\alpha)\iff x_F=\infty\ \text{and}\ \overline F\in\mathrm{RV}_{-\alpha}.}
  $$

  Equivalently $\overline F(tu)/\overline F(t)\to u^{-\alpha}$ for every $u>0$.
- For the [negative Weibull distribution](../../../../../negative-weibull-distribution.md),$$
  \boxed{F\in D(\Psi_\alpha)\iff x_F<\infty\ \text{and}\ t\mapsto\overline F(x_F-1/t)\in\mathrm{RV}_{-\alpha}.}
  $$

  Equivalently $\overline F(x_F-su)/\overline F(x_F-s)\to u^\alpha$ as $s\downarrow0$, for every $u>0$.
- For the [Gumbel distribution](../../../../../gumbel-distribution.md),$$
  \boxed{F\in D(\Lambda)\iff\exists a(t)>0:\quad
  \frac{\overline F(t+a(t)x)}{\overline F(t)}\longrightarrow e^{-x}
  \quad(t\uparrow x_F),\quad x\in\mathbb R.}
  $$

  Here $a$ is a [Gumbel auxiliary function](../../../../../gumbel-auxiliary-function.md), and $x_F$ can be finite or infinite. For each fixed $x$, the shifted argument lies below $x_F$ eventually. This exponential tail-ratio condition, rather than [regular variation](../../../../../regular-variation.md) with a fixed finite index, characterizes this case.

For the corresponding sufficient [hazard function](../../../../../hazard-function.md) conditions, assume $F$ is absolutely continuous near $x_F$, its [survival function](../../../../../survival-function.md) tends to zero there, and its [probability density function](../../../../../probability-density-function.md) $f$ is positive there. Write $\eta(t)=f(t)/\overline F(t)$. The [Von Mises conditions for extreme values](../../../../../von-mises-conditions-for-extreme-values.md) give

$$
\boxed{\begin{array}{ll}
x_F=\infty,\quad t\eta(t)\to\alpha
&\Longrightarrow F\in D(\Phi_\alpha),\\[2pt]
x_F<\infty,\quad(x_F-t)\eta(t)\to\alpha
&\Longrightarrow F\in D(\Psi_\alpha),\\[2pt]
\displaystyle\frac{d}{dt}\left(\frac1{\eta(t)}\right)\to0
&\Longrightarrow F\in D(\Lambda).
\end{array}}
$$

The last condition additionally assumes that the reciprocal [hazard function](../../../../../hazard-function.md) is continuously differentiable near the endpoint. It concerns the derivative of the reciprocal [hazard function](../../../../../hazard-function.md), not the derivative of the [hazard function](../../../../../hazard-function.md) itself. Equivalently, when $f$ is differentiable, it is $\overline F(t)f'(t)/f(t)^2\to-1$.

To see the connection, taking an [integral](../../../../../integral.md) of the [hazard function](../../../../../hazard-function.md) gives

$$
\log\frac{\overline F(v)}{\overline F(t)}=-\int_t^v\eta(u)\,du.
$$

The first two limits make the logarithmic tail ratios over multiplicative or endpoint-distance intervals tend to $-\alpha\log u$ or $\alpha\log u$, giving the required [regular variation](../../../../../regular-variation.md). For the [Gumbel distribution](../../../../../gumbel-distribution.md), set $a(t)=1/\eta(t)$. The derivative condition makes $a(t+a(t)v)/a(t)\to1$ uniformly on bounded $v$-intervals, so

$$
\log\frac{\overline F(t+a(t)x)}{\overline F(t)}
=-\int_0^x\frac{a(t)}{a(t+a(t)v)}\,dv\longrightarrow-x.
$$

The endpoint assumptions ensure these shifts are admissible: at an infinite endpoint $a(t)/t\to0$, and at a finite endpoint $a(t)/(x_F-t)\to0$. These are sufficient smooth-tail conditions; the tail-ratio characterizations above are necessary and sufficient without differentiability assumptions. For a source using the same reciprocal-hazard convention, see [Smith and Weissman's university lecture notes, equations (2.18)–(2.24)](https://rls.sites.oasis.unc.edu/s834-2020/ExtremeValues.pdf#page=12).

For the [Gamma distribution](../../../../../gamma-distribution.md) with integer shape $m$ and rate one, let $\overline F_m(t)=\int_t^\infty u^{m-1}e^{-u}\,du/(m-1)!$. The base case is $\overline F_1(t)=e^{-t}$, and [integration by parts](../../../../../integration-by-parts.md) gives

$$
\overline F_m(t)=\frac{t^{m-1}e^{-t}}{(m-1)!}+\overline F_{m-1}(t).
$$

Induction proves

$$
\boxed{1-F_m(t)=e^{-t}\sum_{j=0}^{m-1}\frac{t^j}{j!},\qquad t\geq0.}
$$

This [survival function](../../../../../survival-function.md) has the asymptotic form $\overline F_m(t)\sim e^{-t}t^{m-1}/(m-1)!$; for $m=1$ the relation is exact. Put $t_n=\beta_n+x$. For every fixed real $x$, $t_n\to\infty$ and $t_n/\log n\to1$. The proposed centering satisfies

$$
n e^{-\beta_n}=\frac{(m-1)!}{(\log n)^{m-1}},
$$

so

$$
n\overline F_m(\beta_n+x)
=e^{-x}\frac{(m-1)!}{(\log n)^{m-1}}
\sum_{j=0}^{m-1}\frac{(\beta_n+x)^j}{j!}
\longrightarrow e^{-x}.
$$

Only the highest-degree term contributes to the limit, with the same reasoning covering $m=1$. The [Taylor expansion](../../../../../taylor-expansion.md) $\log(1-u)=-u+O(u^2)$ now gives

$$
n\log F_m(\beta_n+x)\longrightarrow-e^{-x},
$$

because $n\overline F_m(\beta_n+x)^2\to0$. Therefore the [Gumbel limit for gamma maxima](../../../../../gumbel-limit-for-gamma-maxima.md) is

$$
\boxed{F_m(\beta_n+x)^n\longrightarrow\exp(-e^{-x}),\qquad x\in\mathbb R.}
$$

Equivalently, $M_n-\beta_n$ has [convergence in distribution](../../../../../convergence-in-distribution.md) to the standard [Gumbel distribution](../../../../../gumbel-distribution.md), with scale $a_n=1$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
