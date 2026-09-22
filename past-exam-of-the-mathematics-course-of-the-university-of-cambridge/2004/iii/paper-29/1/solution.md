<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $\theta>0$, the [one-parameter Poisson-Dirichlet distribution](../../../../../one-parameter-poisson-dirichlet-distribution.md) is a [probability distribution](../../../../../probability-distribution.md) on decreasing random mass sequences. A precise construction uses a [Poisson random measure](../../../../../poisson-random-measure.md) $\Xi$ on $(0,\infty)$ with intensity

$$
\rho_\theta(du)=\theta u^{-1}e^{-u}\,du.
$$

Arrange its points as $J_1>J_2>\cdots$ and put $T=\sum_iJ_i$. The intensity is diffuse, so there are [almost surely](../../../../../almost-sure-convergence.md) no ties. There are infinitely many points because the intensity has infinite mass near zero, but their sum is finite [almost surely](../../../../../almost-sure-convergence.md): the [Campbell first-moment formula](../../../../../campbell-first-moment-formula.md) gives $\mathbb ET=\int u\rho_\theta(du)=\theta<\infty$. Also $T>0$ [almost surely](../../../../../almost-sure-convergence.md), since the [probability](../../../../../probability.md) of having no points is zero. Define

$$
\boxed{p_i=J_i/T,\qquad p_1\ge p_2\ge\cdots>0,\qquad\sum_i p_i=1.}
$$

Its law is $PD(\theta)$, also written $PD(0,\theta)$. In particular, $p_1$ is the largest component; the ordering is part of the definition.

The [Laplace functional of a Poisson random measure](../../../../../laplace-functional-of-a-poisson-random-measure.md) determines the total:

$$
\mathbb E e^{-sT}
=\exp\left[-\theta\int_0^\infty\frac{e^{-u}-e^{-(1+s)u}}{u}\,du\right]
=(1+s)^{-\theta},\qquad s\ge0.
$$

For the integral identity, differentiate the integral with respect to $s$, obtaining $1/(1+s)$, and use its value zero at $s=0$. Thus $T$ has the [Gamma distribution](../../../../../gamma-distribution.md) with shape $\theta$ and rate one, and density $t^{\theta-1}e^{-t}/\Gamma(\theta)$.

We use the [Mecke formula for a Poisson random measure](../../../../../mecke-formula-for-a-poisson-random-measure.md) in its point-removal form

$$
\mathbb E\sum_{u\in\Xi}H(u,\Xi-\delta_u)
=\int_0^\infty\mathbb EH(u,\Xi)\,\rho_\theta(du).
$$

Here the process inside the [expectation](../../../../../expected-value.md) on the right has the original law. To justify this identity, first take finite intensity. Conditional on a Poisson count $n$, its points are [independent](../../../../../independent-random-variables.md) samples from normalized intensity. Expanding the [expectation](../../../../../expected-value.md) as a sum over $n$ and singling out one of the $n$ points replaces $n/n!$ by $1/(n-1)!$; the remaining points have the original Poisson law. For sigma-finite intensity, restrict the selected point to a finite-intensity set, condition on the [independent](../../../../../independent-random-variables.md) outside process, and then exhaust the space. [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) proves the formula for nonnegative $H$; absolute integrability allows signed $H$.

Apply it with $H(u,\eta)=\varphi(u/(u+\int v\eta(dv)))$. For the [polynomial](../../../../../polynomial-split.md) in question, $|\varphi(x)|\le Cx$ on $[0,1]$, so $\sum_i|\varphi(p_i)|\le C$ and all signed interchanges are justified. Integrating over the gamma law of the remaining total gives

$$
\mathbb E\sum_i\varphi(p_i)
=\frac{\theta}{\Gamma(\theta)}
\int_0^\infty\int_0^\infty
\varphi\left(\frac{u}{u+t}\right)u^{-1}t^{\theta-1}e^{-(u+t)}\,dt\,du.
$$

Set $s=u+t$ and $x=u/s$, so $u=sx$, $t=s(1-x)$ and the Jacobian is $s$. The integrand factors as $\varphi(x)x^{-1}(1-x)^{\theta-1}s^{\theta-1}e^{-s}$. The integral defining the [Gamma function](../../../../../gamma-function.md) cancels $\Gamma(\theta)$, yielding

$$
\boxed{\mathbb E\sum_i\varphi(p_i)
=\theta\int_0^1\varphi(x)x^{-1}(1-x)^{\theta-1}\,dx.}
$$

For example, setting $\varphi(x)=x^k$ gives $\mathbb E\sum_i p_i^k=\theta B(k,\theta)=\Gamma(k)\Gamma(\theta+1)/\Gamma(k+\theta)$ for integers $k\ge1$.

The same nonnegative calculation identifies the [mean measure of Poisson-Dirichlet components](../../../../../mean-measure-of-poisson-dirichlet-components.md) for arbitrary nonnegative test functions. Write $N_a=\#\{i:p_i>a\}$. If $1/2\le a<1$, at most one component exceeds $a$, so $N_a=\mathbf1_{\{p_1>a\}}$. Hence the identity directly gives the upper part of the [probability distribution](../../../../../probability-distribution.md) of the [largest component of a Poisson-Dirichlet partition](../../../../../largest-component-of-a-poisson-dirichlet-partition.md):

$$
\boxed{\mathbb P(p_1>a)=\theta\int_a^1 x^{-1}(1-x)^{\theta-1}\,dx\quad(1/2\le a<1).}
$$

Its density on $(1/2,1)$ is $\theta x^{-1}(1-x)^{\theta-1}$. For $\theta=1$, this tail is $-\log a$, and $\mathbb P(p_1>1/2)=\log2$. On the other hand, selecting index $I$ with conditional probabilities $\mathbb P(I=i\mid(p_j))=p_i$ weights the [mean measure of a point process](../../../../../intensity-measure-of-a-point-process.md) by $x$. Thus $p_I$ has density $\theta(1-x)^{\theta-1}$, the $\operatorname{Beta}(1,\theta)$ law of a [size-biased distribution](../../../../../size-biased-distribution.md). That beta law describes the selected component.

For completeness, the whole [probability distribution](../../../../../probability-distribution.md) of $p_1$ can also be specified; below one half the expected count $\mathbb EN_a$ is not itself the tail [probability](../../../../../probability.md). Repeating the point-removal formula for $m$ ordered distinct jumps gives the [factorial moment densities of Poisson-Dirichlet components](../../../../../factorial-moment-densities-of-poisson-dirichlet-components.md):

$$
\alpha_\theta^{(m)}(dx_1\cdots dx_m)
=\theta^m\frac{(1-x_1-\cdots-x_m)^{\theta-1}}{x_1\cdots x_m}\,dx_1\cdots dx_m,
\qquad x_i>0,\quad\sum_i x_i<1.
$$

Indeed, integrate over $m$ selected jumps $u_i$ and the remaining gamma total $t$, then put $s=t+\sum_i u_i$, $x_i=u_i/s$. The Jacobian is $s^m$; the factors $\prod_i u_i^{-1}t^{\theta-1}$ and the Jacobian leave $s^{\theta-1}$, whose [Gamma function](../../../../../gamma-function.md) again cancels the normalizing constant. Since $N_a<1/a$, the finite binomial identity for the indicator of $N_a=0$ now gives, for $0<a<1$,

$$
\boxed{\mathbb P(p_1\le a)
=\sum_{m=0}^{\lfloor1/a\rfloor}\frac{(-\theta)^m}{m!}
\int_{\substack{x_i>a\\x_1+\cdots+x_m<1}}
\frac{(1-x_1-\cdots-x_m)^{\theta-1}}{x_1\cdots x_m}\,dx_1\cdots dx_m.}
$$

The $m=0$ term is one; an empty integration region contributes zero. This is [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md), since $\mathbf1_{\{N_a=0\}}=\sum_m(-1)^m(N_a)_m/m!$. Extend this [cumulative distribution function](../../../../../cumulative-distribution-function.md) by zero for $a\le0$ and one for $a\ge1$. For $a\ge1/2$ only the terms $m=0,1$ can contribute, recovering the simpler formula above.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
