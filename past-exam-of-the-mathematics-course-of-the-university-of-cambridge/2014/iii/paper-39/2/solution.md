<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $w_m=w(m/n)$, so a type $v$ values a prize at $v w_m$. In a symmetric increasing [Bayes-Nash equilibrium](../../../../../bayesian-nash-equilibrium.md) of this [rank-order contest](../../../../../rank-order-contest.md), a player reporting type $t$ wins when at most $m-1$ opponents have larger types. Its [winning probability](../../../../../winning-probability.md) is

$$
q_m(t)=\sum_{j=0}^{m-1}\binom{n-1}{j}(1-t)^j t^{n-1-j}.
$$

Here the count of opponents above $t$ has a [binomial distribution](../../../../../binomial-distribution.md). Differentiation, or the associated [order statistic](../../../../../order-statistic.md) density, gives

$$
q_m'(t)=\frac{(n-1)!}{(n-m-1)!(m-1)!}\,t^{n-m-1}(1-t)^{m-1}.
$$

Define the effort by the [all-pay effort identity](../../../../../all-pay-effort-identity.md)

$$
\boxed{b(v)=w_m\int_0^v t q_m'(t)\,dt.}
$$

This also verifies equilibrium globally. The derivative of a type $v$'s payoff from reporting $t$ is $w_m(v-t)q_m'(t)$, positive before $v$ and negative after $v$. Thus truthful reporting is a [best response](../../../../../best-response.md). Bidding above the maximal equilibrium effort gains no additional [winning probability](../../../../../winning-probability.md). Type zero chooses zero effort.

By exchanging the two integrations, the [expected value](../../../../../expected-value.md) of total effort is

$$
\begin{aligned}
R_m&=n\int_0^1b(v)\,dv
=nw_m\int_0^1t(1-t)q_m'(t)\,dt\\
&=\boxed{\frac{m(n-m)}{n+1}\,w(m/n).}
\end{aligned}
$$

The last integral is the moment $\mathbb E[X(1-X)]$ for a [Beta distribution](../../../../../beta-distribution.md) with parameters $n-m$ and $m$, namely $m(n-m)/(n(n+1))$. This is the [uniform-value multi-prize all-pay effort formula](../../../../../uniform-value-multi-prize-all-pay-effort-formula.md).

Put $x=m/n$ and $h(x)=w(x)x(1-x)$. The positive constant $n^2/(n+1)$ multiplying $h(x)$ does not affect the maximizing $m$. Since

$$
h'(x)=w'(x)x(1-x)+w(x)(1-2x),
$$

the assumed inequality makes $h$ nonincreasing on the feasible interval. Hence **one prize maximizes expected total effort**.

For the power family, the PDF gives $w(x)=x^{-\alpha}$. Then

$$
h(x)=x^{1-\alpha}(1-x),\qquad
h'(x)=x^{-\alpha}\bigl[(1-\alpha)-(2-\alpha)x\bigr].
$$

If $\alpha\geq1$, this derivative is strictly negative for $0<x<1$: the bracket is affine and its values at the endpoints are $1-\alpha\leq0$ and $-1$. Thus **$m=1$ is optimal**.

If $0<\alpha<1$, the unique continuous maximizer is

$$
\boxed{x_* =\frac{1-\alpha}{2-\alpha}.}
$$

The objective strictly increases before $x_*$ and decreases after it. Therefore its discrete maximizer lies among

$$
\boxed{\left\{\lfloor nx_*\rfloor,\ \lfloor nx_*\rfloor+1\right\}\cap\{1,\ldots,n-1\}.}
$$

Compare the surviving candidates using $m^{1-\alpha}(n-m)$, since $R_m=n^\alpha m^{1-\alpha}(n-m)/(n+1)$. If $nx_*$ is an integer, that integer is the unique maximizer; if its floor is zero, the only feasible candidate is $1$. This proves the [discrete prize-count optimization for a power-valued contest](../../../../../discrete-prize-count-optimization-for-a-power-valued-contest.md) including the endpoint cases.

The sufficient condition need only hold on $[1/n,(n-1)/n]$. The power family is undefined at zero, so the printed endpoint $x=0$ cannot apply to it. More generally, a positive finite value $w(0)$ would make the displayed inequality fail at zero. The design argument uses only positive feasible prize fractions and needs no value there.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
