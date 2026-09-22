# Roth density-increment step

↑ **Parent:** [Density increment](density-increment.md)

There is an absolute constant $c>0$ such that, for every $\delta>0$ and all sufficiently large $N$, a subset $A\subseteq[N]$ whose [density of a finite subset](density-of-a-finite-subset.md) is $\delta$ and which has no nonconstant three-term [arithmetic progression](arithmetic-progression.md) has an [arithmetic progression](arithmetic-progression.md) $P\subseteq[N]$ satisfying

$$
|P|\geq\eta(\delta)\sqrt N,
\qquad
\frac{|A\cap P|}{|P|}\geq\delta+c\delta^2.
$$

The [Fourier transform](fourier-transform.md) of the balanced function $f=1_A-\delta1_{[N]}$ has a coefficient of magnitude at least $c_0\delta^2N$. Indeed, the trilinear count

$$
\Lambda(g_1,g_2,g_3)=\sum_{x+z=2y}g_1(x)g_2(y)g_3(z)
$$

satisfies $\Lambda(1_A,1_A,1_A)=|A|$, whereas $\Lambda(1_{[N]},1_{[N]},1_{[N]})\gg N^2$. Expanding $1_A=\delta1_{[N]}+f$ and using the [Parseval identity](parseval-identity.md) and the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) to bound every error term forces $\|\widehat f\|_\infty\gg\delta^2N$ once $N$ is sufficiently large in terms of $\delta$.

Choose $\theta$ at which this large coefficient occurs. The [Dirichlet approximation theorem](dirichlet-s-approximation-theorem.md) gives $1\leq d\leq\sqrt N$ with $\|d\theta\|_{\mathbb R/\mathbb Z}\leq N^{-1/2}$. Partition $[N]$ into progressions of common difference $d$ and lengths between $\eta\sqrt N$ and $2\eta\sqrt N$, where $\eta>0$ is a sufficiently small multiple of $\delta^2$. The [linear phase](linear-phase.md) $e(\theta x)$ varies by $O(\eta)$ on each cell. The large Fourier coefficient then gives

$$
\sum_P\left|\sum_{x\in P}f(x)\right|\gg\delta^2N.
$$

Since $\sum_{x\in[N]}f(x)=0$, the total positive discrepancy is half the total absolute discrepancy, so at least one cell has average of $f$ at least $c\delta^2$. This is the required density increment.

**Table of contents**

- [One-frequency density increment on an integer interval](one-frequency-density-increment-on-an-integer-interval.md)
- [Fourier detection of a progression-free subset of an interval](fourier-detection-of-a-progression-free-subset-of-an-interval.md)

## ↑ Ancestors (6)

1. [Density increment](density-increment.md)
2. [Additive combinatorics](additive-combinatorics-split.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Classical Roth bound for three-term progressions](classical-roth-bound-for-three-term-progressions.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-147/2/solution.md)
- [Roth theorem on three-term arithmetic progressions](roth-theorem-on-three-term-arithmetic-progressions.md)
