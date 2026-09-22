<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

First prove the [Baire category theorem](../../../../../baire-category-theorem.md) in its complete-metric form. Let $X$ be a nonempty [complete metric space](../../../../../complete-metric-space.md), let $G_n$ be open [dense sets](../../../../../dense-set.md), and let $V$ be any nonempty [open set](../../../../../open-set.md). Choose a closed ball $\overline B(x_1,r_1)\subset V\cap G_1$ with $0<r_1<1/2$. Inductively, density and openness permit the choice

$$
\overline B(x_{n+1},r_{n+1})\subset B(x_n,r_n)\cap G_{n+1},\qquad 0<r_{n+1}<2^{-(n+1)}.
$$

For $m>n$, $x_m$ belongs to the $n$th closed ball, so $d(x_m,x_n)\le r_n$. The centers form a [Cauchy sequence](../../../../../cauchy-sequence.md) and converge to some $x\in X$ by completeness. Each closed ball contains all later centers and therefore contains their limit. Hence $x\in V\cap\bigcap_nG_n$. Since this holds for every $V$, **every countable intersection of open dense sets is dense**. Equivalently, a nonempty [complete metric space](../../../../../complete-metric-space.md) cannot be a countable union of closed sets with empty interior; this is the form needed below.

For the [Banach-Steinhaus theorem](../../../../../uniform-boundedness-principle.md), let $X$ be a [Banach space](../../../../../banach-space-split.md), $Y$ a [normed vector space](../../../../../normed-vector-space.md), and $\mathcal T$ a family of [bounded linear operators](../../../../../continuous-linear-operator.md) from $X$ to $Y$ such that $\sup_{T\in\mathcal T}\|Tx\|<\infty$ for every $x$. Define

$$
E_m=\{x\in X:\|Tx\|\le m\text{ for every }T\in\mathcal T\},\qquad m=1,2,\ldots.
$$

Each $E_m$ is closed, as an intersection of inverse images of closed balls under continuous maps, and pointwise boundedness gives $X=\bigcup_mE_m$. The [Baire category theorem](../../../../../baire-category-theorem.md) gives some $E_m$ with nonempty interior. Choose $B(x_0,r)\subset E_m$. If $\|h\|\le r/2$, both $x_0+h$ and $x_0$ lie in $E_m$, so $\|Th\|\le2m$ for every $T$. Applying this to $h=(r/2)u$ with $\|u\|\le1$ proves

$$
\boxed{\sup_{T\in\mathcal T}\|T\|\le\frac{4m}{r}<\infty.}
$$

This proves the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md); completeness is required for the domain, but not for $Y$.

Now fix the prescribed point $\theta_0$ on the [unit circle](../../../../../complex-unit-circle.md), parametrized by angles modulo $2\pi$. On the real [Banach space](../../../../../banach-space-split.md) $C(\mathbb T;\mathbb R)$ with the [supremum norm](../../../../../supremum-norm.md), consider the [continuous linear functionals](../../../../../continuous-linear-functional.md) $T_Nf=S_Nf(\theta_0)$, where $S_N$ is the symmetric [Fourier partial sum](../../../../../fourier-partial-sum.md). Summing the finite [geometric series](../../../../../geometric-series.md) gives its [Dirichlet kernel](../../../../../dirichlet-kernel.md) representation

$$
T_Nf=\frac1{2\pi}\int_{-\pi}^{\pi}f(\theta_0-t)D_N(t)\,dt,\qquad D_N(t)=\sum_{j=-N}^Ne^{ijt}=\frac{\sin((N+1/2)t)}{\sin(t/2)}.
$$

The continuous extension at $t=0$ is $2N+1$. The kernel bound gives $\|T_N\|\le\Lambda_N=(2\pi)^{-1}\int|D_N|$. Equality holds: the continuous periodic functions defined by

$$
f_\delta(\theta_0-t)=\frac{D_N(t)}{\sqrt{D_N(t)^2+\delta^2}}
$$

have [supremum norm](../../../../../supremum-norm.md) at most one, and [dominated convergence](../../../../../dominated-convergence-theorem.md) gives $T_Nf_\delta\to\Lambda_N$ as $\delta\downarrow0$.

These norms are unbounded. Indeed, evenness and $\sin(t/2)\le t/2$ for $0<t\le\pi$ give

$$
\Lambda_N\ge\frac2\pi\int_0^{(N+1/2)\pi}\frac{|\sin u|}{u}\,du\ge\frac4{\pi^2}\sum_{j=1}^N\frac1j.
$$

For the second inequality, integrate over $[(j-1)\pi,j\pi]$, where $1/u\ge1/(j\pi)$ and the integral of $|\sin u|$ is two. The [harmonic series](../../../../../harmonic-series.md) diverges, proving the [Dirichlet kernel harmonic lower bound](../../../../../dirichlet-kernel-harmonic-lower-bound.md). If every continuous $f$ had bounded partial sums at $\theta_0$, the [Banach-Steinhaus theorem](../../../../../uniform-boundedness-principle.md) would bound all the operator norms, a contradiction. Consequently **there exists a continuous real function $f$ with $\sup_N|S_Nf(\theta_0)|=\infty$**, and its [Fourier series](../../../../../fourier-series-split.md) diverges at the prescribed point. The function depends on the chosen point; the argument requires no claim of simultaneous divergence everywhere.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
