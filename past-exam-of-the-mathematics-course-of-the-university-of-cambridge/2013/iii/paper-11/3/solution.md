<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We use the normalized [Gowers U3 norm on an interval](../../../../../gowers-u3-norm-on-an-interval.md), for which a [quadratic phase](../../../../../quadratic-phase.md) has norm one. Let $\mathcal C_N$ consist of integer tuples $(x,h_1,h_2,h_3)$ whose eight vertices $x+\omega_1h_1+\omega_2h_2+\omega_3h_3$, $\omega\in\{0,1\}^3$, all lie in $[1,N]$. If $\mathcal C$ denotes complex conjugation, define

$$
\|f\|_{U^3(N)}^8=\frac1{|\mathcal C_N|}\sum_{(x,h_1,h_2,h_3)\in\mathcal C_N}\prod_{\omega\in\{0,1\}^3}\mathcal C^{|\omega|}f(x+\omega\cdot h).
$$

Equivalently, choose a prime $8N<M<16N$, extend $f$ by zero to $G=\mathbb Z/M\mathbb Z$, call that extension $F$, and put $I=\mathbf1_{[1,N]}$. Then

$$
\|f\|_{U^3(N)}=\frac{\|F\|_{U^3(G)}}{\|I\|_{U^3(G)}}.
$$

The large ambient modulus prevents wraparound in cubes supported on the interval, so the ratio is independent of the chosen such $M$. This also proves nonnegativity and the norm properties by the [Gowers uniformity norm](../../../../../gowers-uniformity-norm.md) on $G$. Some conventions omit the denominator; their interval norm differs by a fixed bounded factor, and the quadratic-phase norm is then $\|I\|_{U^3(G)}$.

For $f_0(x)=e(\alpha x^2)$, the exponent in every conjugated cube product is a third additive difference of a quadratic polynomial and is zero. Thus **$\|f_0\|_{U^3(N)}=1$** in the normalized interval convention.

The [generalized von Neumann inequality for four-term progressions](../../../../../generalized-von-neumann-inequality-for-four-term-progressions.md) connects this norm to counting [arithmetic progressions](../../../../../arithmetic-progression.md). For functions bounded by one on a cyclic group of prime order greater than three,

$$
\left|\mathbb E_{x,d}\prod_{j=0}^3g_j(x+jd)\right|\leq\min_j\|g_j\|_{U^3}.
$$

Three applications of [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) prove the bound. Zero extension and division by the number of interval progressions give the analogous interval estimate up to an absolute constant. In particular, if $g=\mathbf1_A-\alpha\mathbf1_{[1,N]}$, where $\alpha=|A|/N$, has small [Gowers U3 norm on an interval](../../../../../gowers-u3-norm-on-an-interval.md), expansion of the progression count shows that it differs from $\alpha^4$ times the count for $[1,N]$ by $O(\|g\|_{U^3(N)}N^2)$. A large [Gowers U3 norm](../../../../../gowers-u3-norm.md) detects structure capable of changing four-term progression counts; [quadratic phases](../../../../../quadratic-phase.md) are the basic example.

For the remaining proof use the ambient $G$ just specified, define $\partial_hF(x)=F(x+h)\overline{F(x)}$, and take averages uniformly on $G$. For frequencies not on the character grid, an exponential is evaluated at the chosen integer representatives; the general proof below selects actual characters $\theta=k/M$. The printed question does not define $G$ or the interval normalization, so these conventions make the assertion precise. If instead $\partial_hf(x)=f(x)\overline{f(x+h)}$ is used, conjugate the correlations and reverse every frequency sign; the quadratic example then has $\theta(h)=-2\alpha h$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
