<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the [Kahane-Katznelson divergence theorem](../../../../../../kahane-katznelson-divergence-theorem.md) through an explicit small-norm block construction. Let $\mu$ be normalized [Lebesgue measure](../../../../../../lebesgue-measure.md) on the circle.

First establish the [compact-set Fourier amplification lemma](../../../../../../compact-set-fourier-amplification-lemma.md). If a compact set $K$ satisfies

$$
\mu(K)\leq\exp(-8\pi M/\varepsilon),\qquad0<\varepsilon\leq1,\quad M\geq1,
$$

we can make a [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) $q$ with $\|q\|_\infty\leq\varepsilon$, supported in any sufficiently high interval of positive frequencies, whose partial prefix has magnitude greater than $M$ on $K$.

To construct it, choose a smooth nonnegative function $u$ equal to one near $K$, with values at most one and mean

$$
0<\delta=\int u\,d\mu<\exp(-4\pi M/\varepsilon).
$$

[Outer regularity](../../../../../../outer-regular-measure.md) and a smooth cutoff give this choice; the stipulated bound on $\mu(K)$ leaves room between the two exponentials. The [Schwarz integral on the unit disk](../../../../../../schwarz-integral-on-the-unit-disk.md)

$$
H(z)=\int_{\mathbb T}\frac{e^{it}+z}{e^{it}-z}\,u(t)\,d\mu(t)
$$

has positive real part in the disk, $H(0)=\delta$, and boundary real part $u$. Its [holomorphic logarithm](../../../../../../holomorphic-logarithm.md)

$$
W(z)=\log H(z)-\log\delta
$$

satisfies $W(0)=0$ and $|\operatorname{Im}W|<\pi/2$. On $K$, the boundary value has $\operatorname{Re}W\geq\log(1/\delta)>4\pi M/\varepsilon$. Smoothness of $u$ makes $H$ continuous at the boundary, and its positive boundary real part near $K$ makes $W$ continuous there.

Choose a radius just below one, then truncate the Taylor series of $W$ at that radius. This gives an analytic polynomial $R(e^{it})$ with zero constant term, degree $d$, and

$$
|\operatorname{Im}R(t)|<\pi,\qquad
\operatorname{Re}R(t)>4\pi M/\varepsilon-1\quad(t\in K).
$$

The radial function is analytic beyond the closed unit disk, so the Taylor truncation is uniform on the whole circle. For $L>d$, put

$$
q(t)=\frac{\varepsilon}{\pi}e^{iLt}\operatorname{Im}R(t).
$$

Its frequencies lie between $L-d$ and $L+d$, all positive. Its prefix through frequency $L$ includes exactly the negative-frequency half of $\operatorname{Im}R$ shifted into this interval:

$$
S_Lq(t)=-\frac{\varepsilon}{2\pi i}e^{iLt}\overline{R(t)}.
$$

Consequently $|S_Lq(t)|>\varepsilon(4\pi M/\varepsilon-1)/(2\pi)>M$ on $K$, whereas $\|q\|_\infty<\varepsilon$. Increasing $L$ places the entire block above any previously used frequency.

We next use [compact batching of a small open set](../../../../../../compact-batching-of-a-small-open-set.md) to handle an arbitrary null set, without assuming that it is compact or a countable union of compact null sets. Set

$$
\varepsilon_{j,k}=2^{-j-k-2},\qquad j\geq1,\ k\geq0.
$$

For each $j$, choose an open $U_j\supseteq E$ with $\mu(U_j)<\exp(-8\pi j/\varepsilon_{j,0})$. Decompose $U_j$ into countably many closed subarcs with pairwise disjoint interiors: subdivide each open component into closed pieces accumulating only at its excluded endpoints. Group these subarcs into finite successive batches $K_{j,k}$. After batch $k$, include enough pieces that the remaining total length is less than $\exp(-8\pi j/\varepsilon_{j,k+1})$. Require each batch endpoint in the enumeration to increase. Then

$$
U_j=\bigcup_{k\geq0}K_{j,k},\qquad
\mu(K_{j,k})\leq\exp(-8\pi j/\varepsilon_{j,k}).
$$

Each batch is compact; endpoints shared by pieces have zero measure and do not affect the estimates.

Enumerate the pairs $(j,k)$ in diagonal order. Apply the block lemma with target $M=j$ to each $K_{j,k}$, and shift its spectrum above all preceding blocks. Denote the resulting polynomial by $q_{j,k}$ and set

$$
f=\sum_{j\geq1,\ k\geq0}q_{j,k}.
$$

Since $\sum_{j,k}\varepsilon_{j,k}=1/2$, this series is uniformly convergent and defines a continuous complex-valued function.

Fix $t\in E$. For every $j$ there is a $k$ with $t\in K_{j,k}$. The difference between the [Fourier partial sum](../../../../../../fourier-partial-sum.md) just before that block and the sum at its midpoint has magnitude greater than $j$: previous blocks cancel in the difference, and future blocks have not yet entered. As $j\to\infty$, these cutoffs tend to infinity. At least one of the two partial sums therefore has magnitude greater than $j/2$. The [Fourier partial sums](../../../../../../fourier-partial-sum.md) are unbounded, hence not Cauchy, at $t$. We have proved

$$
\boxed{E\subseteq\{t:\limsup_N|S_Nf(t)|=\infty\}.}
$$

This establishes divergence on every prescribed null set, including dense nonclosed null sets; it does not assert that the divergence set is exactly $E$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
