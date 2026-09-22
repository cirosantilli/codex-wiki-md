<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Roth theorem on three-term arithmetic progressions](../../../../../roth-theorem-on-three-term-arithmetic-progressions.md) says that, for every $\delta>0$, every sufficiently long integer interval contains a nonconstant three-term [arithmetic progression](../../../../../arithmetic-progression.md) in every subset of [subset density](../../../../../density-of-a-finite-subset.md) at least $\delta$. We prove this by a [density increment](../../../../../density-increment.md), giving the intermediate Fourier and partition arguments.

Let $A\subseteq I=[N]$ have [subset density](../../../../../density-of-a-finite-subset.md) $\alpha>0$ and contain no nonconstant three-term [arithmetic progression](../../../../../arithmetic-progression.md). Embed $I$ in the odd-order [cyclic group](../../../../../cyclic-group.md) $G=\mathbb Z/M\mathbb Z$, where $M=2N+1$, and extend its [indicator function](../../../../../indicator-function.md) by zero. Use normalized [Fourier coefficients on a finite abelian group](../../../../../fourier-coefficient-on-a-finite-abelian-group.md)

$$
\widehat h(r)=\frac1M\sum_{x\in G}h(x)e^{-2\pi irx/M}.
$$

For the normalized progression count,

$$
T(h_1,h_2,h_3)=\frac1{M^2}\sum_{x+z=2y}h_1(x)h_2(y)h_3(z),
$$

the [orthogonality of characters](../../../../../character-orthogonality.md) and [Fourier inversion](../../../../../fourier-inversion-theorem.md) give

$$
T(h_1,h_2,h_3)=\sum_{r\in G}\widehat h_1(r)\widehat h_2(-2r)\widehat h_3(r).
$$

There is no modular wraparound when $x,y,z\in I$, since both $x+z$ and $2y$ lie between $2$ and $2N$. Only constant progressions occur in $A$, so $T(1_A,1_A,1_A)=\alpha N/M^2$. In the interval $I$, endpoints of the same parity have an integer midpoint, giving at least $N^2/2$ ordered progressions.

Put $b=\alpha1_I$ and $f=1_A-b$, so $\widehat f(0)=0$. If $N\ge4\alpha^{-2}$, the difference in progression counts satisfies

$$
T(b,b,b)-T(1_A,1_A,1_A)\ge\frac{\alpha^3N^2}{4M^2}.
$$

Telescope the difference in the other order as $T(f,1_A,1_A)+T(b,f,1_A)+T(b,b,f)$. By [Parseval identity](../../../../../parseval-identity.md) and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), each term has [absolute value](../../../../../absolute-value.md) at most

$$
\|\widehat f\|_\infty\,\frac{\alpha N}{M}.
$$

Indeed $\|1_A\|_2^2=\alpha N/M$, $\|b\|_2^2=\alpha^2N/M$, and multiplication by $-2$ permutes the frequencies because $M$ is odd. It follows that a nonzero frequency $r$ satisfies

$$
|\widehat f(r)|\ge\frac{\alpha^2N}{12M}\ge\frac{\alpha^2}{36}=:\beta.
$$

Thus the unnormalized Fourier correlation has [absolute value](../../../../../absolute-value.md) at least $\beta N$.

Write $\theta=r/M$ and $q=\lfloor\sqrt N\rfloor$. To prove the needed case of the [Dirichlet approximation theorem](../../../../../dirichlet-s-approximation-theorem.md), place the $q+1$ fractional parts $0,\theta,\ldots,q\theta$ in $q$ equal subintervals of $[0,1)$. The [pigeonhole principle](../../../../../pigeonhole-principle.md) gives $1\le d\le q$ with $\|d\theta\|_{\mathbb R/\mathbb Z}\le1/q$. Set $\eta=\beta/(16\pi)$ and $L=\lfloor\eta q\rfloor$, taking $N$ large enough that $\eta q\ge2$. Every residue-class chain in $[N]$ of step $d$ has length at least $q$. Divide each chain into blocks of length $L$, adjoining a final shorter remainder to its preceding block. This partitions $I$ into [arithmetic progressions](../../../../../arithmetic-progression.md) $P$ with $L\le|P|<2L$.

The [linear phase](../../../../../linear-phase.md) $e^{-2\pi i\theta x}$ varies by at most $4\pi L/q\le\beta/4$ on each cell. Replace it there by its value at one endpoint. Since $|f(x)|\le1$, the total error in the Fourier correlation is at most $\beta N/4$. Consequently, writing $D(P)=\sum_{x\in P}f(x)$,

$$
\sum_P|D(P)|\ge\frac{3\beta N}{4}.
$$

But $\sum_PD(P)=0$, so the positive discrepancies sum to at least $3\beta N/8$. Some cell therefore has $D(P)/|P|\ge3\beta/8\ge\beta/4$. As $q\ge\sqrt N/2$ and $L\ge\eta q/2$, this proves the [one-frequency density increment on an integer interval](../../../../../one-frequency-density-increment-on-an-integer-interval.md):

$$
|P|\ge\frac{\alpha^2}{2304\pi}\sqrt N,\qquad
\frac{|A\cap P|}{|P|}\ge\alpha+\frac{\alpha^2}{144}.
$$

Finally, reindex this [arithmetic progression](../../../../../arithmetic-progression.md) as a new integer interval. An affine reindexing preserves three-term [arithmetic progressions](../../../../../arithmetic-progression.md), so the new subset is again progression-free. Starting with density at least $\delta$, each step raises it by at least $\delta^2/144$ and retains an interval of length at least $c\sqrt N$, where $c=\delta^2/(2304\pi)$.

Let $R(\delta)$ be a size threshold large enough for all the preceding estimates. It works at every later density $\alpha\ge\delta$. Choose $J=\lceil144/\delta^2\rceil$ and initial size at least $(R(\delta)/c^2)^{2^J}$. After $j\le J$ steps the size is at least

$$
c^{2(1-2^{-j})}N^{2^{-j}}\ge c^2N^{2^{-j}}\ge R(\delta).
$$

Thus all $J$ increments are permitted. They would give density at least $\delta+J\delta^2/144>1$, a contradiction. This proves the [Roth theorem on three-term arithmetic progressions](../../../../../roth-theorem-on-three-term-arithmetic-progressions.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
