# Paper 29

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper29.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper29.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For $\theta>0$, the [one-parameter Poisson-Dirichlet distribution](../../../probability-theory.md#one-parameter-poisson-dirichlet-distribution) is a [probability distribution](../../../probability-theory.md#probability-distribution) on decreasing random mass sequences. A precise construction uses a [Poisson random measure](../../../probability-theory.md#poisson-random-measure) $\Xi$ on $(0,\infty)$ with intensity

$$
\rho_\theta(du)=\theta u^{-1}e^{-u}\,du.
$$

Arrange its points as $J_1>J_2>\cdots$ and put $T=\sum_iJ_i$. The intensity is diffuse, so there are [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) no ties. There are infinitely many points because the intensity has infinite mass near zero, but their sum is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence): the [Campbell first-moment formula](../../../probability-theory.md#campbell-first-moment-formula) gives $\mathbb ET=\int u\rho_\theta(du)=\theta<\infty$. Also $T>0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), since the [probability](../../../probability-theory.md#probability) of having no points is zero. Define

$$
\boxed{p_i=J_i/T,\qquad p_1\ge p_2\ge\cdots>0,\qquad\sum_i p_i=1.}
$$

Its law is $PD(\theta)$, also written $PD(0,\theta)$. In particular, $p_1$ is the largest component; the ordering is part of the definition.

The [Laplace functional of a Poisson random measure](../../../probability-theory.md#laplace-functional-of-a-poisson-random-measure) determines the total:

$$
\mathbb E e^{-sT}
=\exp\left[-\theta\int_0^\infty\frac{e^{-u}-e^{-(1+s)u}}{u}\,du\right]
=(1+s)^{-\theta},\qquad s\ge0.
$$

For the integral identity, differentiate the integral with respect to $s$, obtaining $1/(1+s)$, and use its value zero at $s=0$. Thus $T$ has the [Gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) with shape $\theta$ and rate one, and density $t^{\theta-1}e^{-t}/\Gamma(\theta)$.

We use the [Mecke formula for a Poisson random measure](../../../probability-theory.md#mecke-formula-for-a-poisson-random-measure) in its point-removal form

$$
\mathbb E\sum_{u\in\Xi}H(u,\Xi-\delta_u)
=\int_0^\infty\mathbb EH(u,\Xi)\,\rho_\theta(du).
$$

Here the process inside the [expectation](../../../probability-theory.md#expected-value) on the right has the original law. To justify this identity, first take finite intensity. Conditional on a Poisson count $n$, its points are [independent](../../../random-variable.md#independent-random-variables) samples from normalized intensity. Expanding the [expectation](../../../probability-theory.md#expected-value) as a sum over $n$ and singling out one of the $n$ points replaces $n/n!$ by $1/(n-1)!$; the remaining points have the original Poisson law. For sigma-finite intensity, restrict the selected point to a finite-intensity set, condition on the [independent](../../../random-variable.md#independent-random-variables) outside process, and then exhaust the space. [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) proves the formula for nonnegative $H$; absolute integrability allows signed $H$.

Apply it with $H(u,\eta)=\varphi(u/(u+\int v\eta(dv)))$. For the [polynomial](../../../polynomial.md) in question, $|\varphi(x)|\le Cx$ on $[0,1]$, so $\sum_i|\varphi(p_i)|\le C$ and all signed interchanges are justified. Integrating over the gamma law of the remaining total gives

$$
\mathbb E\sum_i\varphi(p_i)
=\frac{\theta}{\Gamma(\theta)}
\int_0^\infty\int_0^\infty
\varphi\left(\frac{u}{u+t}\right)u^{-1}t^{\theta-1}e^{-(u+t)}\,dt\,du.
$$

Set $s=u+t$ and $x=u/s$, so $u=sx$, $t=s(1-x)$ and the Jacobian is $s$. The integrand factors as $\varphi(x)x^{-1}(1-x)^{\theta-1}s^{\theta-1}e^{-s}$. The integral defining the [Gamma function](../../../complex-analysis.md#gamma-function) cancels $\Gamma(\theta)$, yielding

$$
\boxed{\mathbb E\sum_i\varphi(p_i)
=\theta\int_0^1\varphi(x)x^{-1}(1-x)^{\theta-1}\,dx.}
$$

For example, setting $\varphi(x)=x^k$ gives $\mathbb E\sum_i p_i^k=\theta B(k,\theta)=\Gamma(k)\Gamma(\theta+1)/\Gamma(k+\theta)$ for integers $k\ge1$.

The same nonnegative calculation identifies the [mean measure of Poisson-Dirichlet components](../../../probability-theory.md#mean-measure-of-poisson-dirichlet-components) for arbitrary nonnegative test functions. Write $N_a=\#\{i:p_i>a\}$. If $1/2\le a<1$, at most one component exceeds $a$, so $N_a=\mathbf1_{\{p_1>a\}}$. Hence the identity directly gives the upper part of the [probability distribution](../../../probability-theory.md#probability-distribution) of the [largest component of a Poisson-Dirichlet partition](../../../probability-theory.md#largest-component-of-a-poisson-dirichlet-partition):

$$
\boxed{\mathbb P(p_1>a)=\theta\int_a^1 x^{-1}(1-x)^{\theta-1}\,dx\quad(1/2\le a<1).}
$$

Its density on $(1/2,1)$ is $\theta x^{-1}(1-x)^{\theta-1}$. For $\theta=1$, this tail is $-\log a$, and $\mathbb P(p_1>1/2)=\log2$. On the other hand, selecting index $I$ with conditional probabilities $\mathbb P(I=i\mid(p_j))=p_i$ weights the [mean measure of a point process](../../../probability-theory.md#intensity-measure-of-a-point-process) by $x$. Thus $p_I$ has density $\theta(1-x)^{\theta-1}$, the $\operatorname{Beta}(1,\theta)$ law of a [size-biased distribution](../../../probability-theory.md#size-biased-distribution). That beta law describes the selected component.

For completeness, the whole [probability distribution](../../../probability-theory.md#probability-distribution) of $p_1$ can also be specified; below one half the expected count $\mathbb EN_a$ is not itself the tail [probability](../../../probability-theory.md#probability). Repeating the point-removal formula for $m$ ordered distinct jumps gives the [factorial moment densities of Poisson-Dirichlet components](../../../probability-theory.md#factorial-moment-densities-of-poisson-dirichlet-components):

$$
\alpha_\theta^{(m)}(dx_1\cdots dx_m)
=\theta^m\frac{(1-x_1-\cdots-x_m)^{\theta-1}}{x_1\cdots x_m}\,dx_1\cdots dx_m,
\qquad x_i>0,\quad\sum_i x_i<1.
$$

Indeed, integrate over $m$ selected jumps $u_i$ and the remaining gamma total $t$, then put $s=t+\sum_i u_i$, $x_i=u_i/s$. The Jacobian is $s^m$; the factors $\prod_i u_i^{-1}t^{\theta-1}$ and the Jacobian leave $s^{\theta-1}$, whose [Gamma function](../../../complex-analysis.md#gamma-function) again cancels the normalizing constant. Since $N_a<1/a$, the finite binomial identity for the indicator of $N_a=0$ now gives, for $0<a<1$,

$$
\boxed{\mathbb P(p_1\le a)
=\sum_{m=0}^{\lfloor1/a\rfloor}\frac{(-\theta)^m}{m!}
\int_{\substack{x_i>a\\x_1+\cdots+x_m<1}}
\frac{(1-x_1-\cdots-x_m)^{\theta-1}}{x_1\cdots x_m}\,dx_1\cdots dx_m.}
$$

The $m=0$ term is one; an empty integration region contributes zero. This is [inclusion-exclusion](../../../combinatorics.md#inclusion-exclusion-principle), since $\mathbf1_{\{N_a=0\}}=\sum_m(-1)^m(N_a)_m/m!$. Extend this [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) by zero for $a\le0$ and one for $a\ge1$. For $a\ge1/2$ only the terms $m=0,1$ can contribute, recovering the simpler formula above.

## 2

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For $r>0$, let $\kappa_r$ be the [probability](../../../probability-theory.md#probability) law of a seed displacement from its tree. For the literal circular support, it is normalized [arclength](../../../riemannian-geometry.md#arc-length) on $\{u:|u|=r\}$. The conditional [mean measure of a point process](../../../probability-theory.md#intensity-measure-of-a-point-process) is

$$
\boxed{\Lambda_\Pi(A)=\mu\sum_{z\in\Pi}\kappa_r(A-z).}
$$

We prove the conditional Poisson assertion directly by joint [probability generating functions](../../../probability-theory.md#probability-generating-function).

Fix disjoint bounded [measurable](../../../measure-theory.md#measurability) sets $A_1,\ldots,A_k$. For a tree at $z$, put $q_j(z)=\kappa_r(A_j-z)$ and $q_0(z)=1-\sum_jq_j(z)$. Conditional on its seed count, the allocation among these sets and their complement is [multinomial distribution](../../../discrete-probability-distribution.md#multinomial-distribution). Averaging over the Poisson seed count gives

$$
\mathbb E\left[\prod_{j=1}^k s_j^{N_z(A_j)}\,\middle|\,\Pi\right]
=\exp\left[\mu\left(q_0(z)+\sum_jq_j(z)s_j-1\right)\right]
=\prod_{j=1}^k\exp\bigl(\mu q_j(z)(s_j-1)\bigr).
$$

Thus this tree contributes [independent](../../../random-variable.md#independent-random-variables) Poisson counts of means $\mu q_j(z)$ to the disjoint sets. Different trees contribute independently. Only trees within distance $r$ of the bounded union of the $A_j$ can contribute, and there are [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) finitely many of them. Multiplying their [probability generating functions](../../../probability-theory.md#probability-generating-function) gives

$$
\mathbb E\left[\prod_j s_j^{\Pi^*(A_j)}\,\middle|\,\Pi\right]
=\prod_j\exp\bigl(\Lambda_\Pi(A_j)(s_j-1)\bigr).
$$

This is precisely the joint [probability generating function](../../../probability-theory.md#probability-generating-function) of [independent](../../../random-variable.md#independent-random-variables) Poisson counts with the displayed means. Also $\Lambda_\Pi$ is locally finite, because each bounded set can receive seeds from only finitely many trees. This proves the conditional [Poisson point process](../../../probability-theory.md#poisson-point-process) assertion and the [Poisson offspring clusters directed by their parent process](../../../probability-theory.md#poisson-offspring-clusters-directed-by-their-parent-process) construction.

In [arclength](../../../riemannian-geometry.md#arc-length) notation the directing measure is $\Lambda_\Pi=\mu\sum_{z\in\Pi}\sigma_{z,r}/(2\pi r)$, where $\sigma_{z,r}$ is [arclength](../../../riemannian-geometry.md#arc-length) on the circle centered at $z$. If “circle” is used to mean the filled disc instead, take $\kappa_r(du)=\mathbf1_{\{|u|\le r\}}du/(\pi r^2)$; then

$$
\Lambda_\Pi(dx)=\frac{\mu}{\pi r^2}\sum_{z\in\Pi}\mathbf1_{\{|x-z|\le r\}}\,dx.
$$

The generating-function proof and the following unconditional conclusion hold for either reading. The circular version has a singular conditional directing measure, giving the [random directing measure of a Cox process](../../../probability-theory.md#random-directing-measure-of-a-cox-process) formulation.

Unconditionally this is a [Cox process](../../../probability-theory.md#cox-process), specifically a Poisson-offspring [Neyman-Scott process](../../../probability-theory.md#neyman-scott-process). Its [mean measure of a point process](../../../probability-theory.md#intensity-measure-of-a-point-process) is nevertheless spatially uniform. With $q_A(z)=\kappa_r(A-z)$, the [Campbell first-moment formula](../../../probability-theory.md#campbell-first-moment-formula) and translation invariance give

$$
\mathbb E\Lambda_\Pi(A)=\lambda\mu\int_{\mathbb R^2}q_A(z)\,dz
=\lambda\mu|A|,
$$

since $\int q_A(z)dz=\int\kappa_r(du)\int\mathbf1_A(z+u)dz=|A|$. Uniform mean alone does not establish a Poisson law.

For a bounded set $A$ of positive area, the conditional count has mean and [variance](../../../variance.md) $\Lambda_\Pi(A)$. The [law of total variance](../../../probability-theory.md#law-of-total-variance) gives

$$
\operatorname{Var}\Pi^*(A)=\mathbb E\Lambda_\Pi(A)+\operatorname{Var}\Lambda_\Pi(A).
$$

A Poisson integral of a deterministic function $q$ has [variance](../../../variance.md) $\lambda\int q^2dz$: for a simple function on disjoint sets this follows from [independent](../../../random-variable.md#independent-random-variables) Poisson counts, and square-integrable approximation gives the general formula. Here $0\le q_A\le1$ and it has bounded support, so

$$
\boxed{\operatorname{Var}\Pi^*(A)
=\lambda\mu|A|+\lambda\mu^2\int_{\mathbb R^2}q_A(z)^2\,dz
>\lambda\mu|A|=\mathbb E\Pi^*(A).}
$$

The strict inequality holds when $\lambda,\mu>0$, because $\int q_A=|A|>0$ implies $\int q_A^2>0$. A Poisson [random variable](../../../random-variable.md) has equal mean and [variance](../../../variance.md). Hence **the unconditional process is not a [Poisson process](../../../probability-theory.md#poisson-process) in the nontrivial model**. If $\lambda=0$ or $\mu=0$, there are no seeds and the process is the degenerate empty [Poisson process](../../../probability-theory.md#poisson-process). The [overdispersion of nondegenerate mixed Poisson counts](../../../discrete-probability-distribution.md#overdispersion-of-nondegenerate-mixed-poisson-counts) quantifies the additional clustering induced by the random parents.

## 3

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $\sigma$ denote [surface measure on a sphere](../../../geometry-and-topology.md#surface-measure-on-a-sphere) on $S^2$ and $\nu$ volume measure on the unit ball. The [Poisson mapping theorem](../../../probability-theory.md#poisson-mapping-theorem) can be proved directly here: counts of image points in disjoint sets are counts of the original process in their disjoint preimages. They are therefore [independent](../../../random-variable.md#independent-random-variables) Poisson variables, and their means are the volumes of those preimages.

For the radius map, a [measurable](../../../measure-theory.md#measurability) set $A\subset[0,1]$ has mean

$$
\boxed{\nu_1(A)=\int_A4\pi r^2\,dr,\qquad
\nu_1([0,a])=\frac{4\pi a^3}{3}\quad(0\le a\le1).}
$$

This follows from [spherical coordinates](../../../calculus.md#spherical-coordinate-system) or by subtracting concentric-ball volumes. The disjoint-preimage argument proves that the radius image is a [Poisson process](../../../probability-theory.md#poisson-process) with this [mean measure of a point process](../../../probability-theory.md#intensity-measure-of-a-point-process). There is no mass at zero or at one.

The original process has no point at the origin [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), since its mean count there is zero. Thus division by $r$ in the direction map is well-defined [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). For a [measurable](../../../measure-theory.md#measurability) surface set $C\subset S^2$, [spherical coordinates](../../../calculus.md#spherical-coordinate-system) give

$$
\boxed{\nu_2(C)=\int_C\int_0^1r^2\,dr\,\sigma(d\omega)=\frac{\sigma(C)}3.}
$$

Again disjoint surface sets have disjoint cone preimages, giving the required [independent](../../../random-variable.md#independent-random-variables) Poisson counts. Both [pushforward measures](../../../measure-theory.md#pushforward-measure) are diffuse, so there are [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) no image collisions; they describe the indicated point sets as well as [counting measures](../../../measure-theory.md#counting-measure).

**The two image processes are not [independent](../../../random-variable.md#independent-random-variables).** They have exactly the same total number of points,

$$
N=\Pi_1([0,1])=\Pi_2(S^2)=\Pi(B)\sim\operatorname{Pois}(4\pi/3).
$$

Indeed,

$$
\mathbb P(\Pi_1=\varnothing,\Pi_2=\varnothing)=e^{-4\pi/3}
\ne e^{-8\pi/3}
=\mathbb P(\Pi_1=\varnothing)\mathbb P(\Pi_2=\varnothing).
$$

This alone disproves process [independence](../../../random-variable.md#independent-random-variables).

More generally, split the original points into those whose radius lies in $A$ and direction lies in $C$, those satisfying only the first condition, and those satisfying only the second. Counts in these three disjoint regions are [independent](../../../random-variable.md#independent-random-variables). The count shared by both images is Poisson with mean $\sigma(C)\int_A r^2dr$, so

$$
\operatorname{Cov}\bigl(\Pi_1(A),\Pi_2(C)\bigr)=\sigma(C)\int_A r^2\,dr.
$$

The fact that [Poisson polar projections share their total count](../../../probability-theory.md#poisson-polar-projections-share-their-total-count) explains the dependence despite the product polar intensity $r^2dr\,\sigma(d\omega)$. Conditional on $N$, the points are [independent](../../../random-variable.md#independent-random-variables) uniform samples from the ball. Their radius density is $3r^2$ and their direction law is $\sigma/(4\pi)$, independently for each point. Thus the two image configurations are [independent](../../../random-variable.md#independent-random-variables) conditional on $N$; unconditionally the shared nonconstant count couples them.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
