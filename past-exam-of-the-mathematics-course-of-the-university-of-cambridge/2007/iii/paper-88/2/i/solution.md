<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A quantitative form of [Roth theorem on three-term arithmetic progressions](../../../../../../roth-theorem-on-three-term-arithmetic-progressions.md) is: there is an absolute constant $C_R$ such that, for $N\geq3$, every $A\subseteq[N]$ with no nonconstant three-term [arithmetic progression](../../../../../../arithmetic-progression.md) satisfies

$$
\boxed{|A|\leq C_R\frac{N}{\log\log N}.}
$$

All logarithms below are natural. We prove the [classical Roth bound for three-term progressions](../../../../../../classical-roth-bound-for-three-term-progressions.md) with an unoptimized $C_R=100$. The empty [set](../../../../../../set-split.md) is immediate; write $\delta=|A|/N>0$.

First establish a quantitative [density increment](../../../../../../density-increment.md). Suppose $N\geq4\cdot10^6\delta^{-4}$. Put $M=2N+1$, embed $I=[N]$ in $G=\mathbb Z_M$, and extend all interval [functions](../../../../../../function-split.md) by zero. Let $a=1_A$, $u=\delta1_I$ and $f=a-u$, the [balanced subset indicator](../../../../../../balanced-indicator-function-of-a-finite-subset.md). Define

$$
\widehat g(r)=\sum_{x\in G}g(x)e^{-2\pi irx/M},\qquad\Lambda(g_1,g_2,g_3)=\sum_{x+z=2y}g_1(x)g_2(y)g_3(z).
$$

The relation in the sum is modulo $M$. For interval elements its [integer](../../../../../../integer.md) discrepancy has absolute value less than $M$, so it is precisely the [integer](../../../../../../integer.md) relation. Thus $\Lambda(a,a,a)=|A|=\delta N$. The full interval count is the number of endpoint pairs of the same parity:

$$
\Lambda(1_I,1_I,1_I)=\lceil N/2\rceil^2+\lfloor N/2\rfloor^2\geq N^2/2.
$$

Consequently, since $N\geq4\delta^{-2}$,

$$
\Lambda(u,u,u)-\Lambda(a,a,a)\geq\frac{\delta^3N^2}{4}.
$$

Orthogonality of the [additive characters](../../../../../../additive-character.md) gives

$$
\Lambda(g_1,g_2,g_3)=\frac1M\sum_r\widehat g_1(r)\widehat g_2(-2r)\widehat g_3(r),\qquad\frac1M\sum_r|\widehat g(r)|^2=\sum_x|g(x)|^2.
$$

Both identities follow by expanding the sums and using $\sum_re^{2\pi irt/M}=M$ for $t=0$ in $G$, and zero otherwise; the latter follows from a [finite geometric series](../../../../../../finite-geometric-series.md). Since $M$ is odd, $r\mapsto-2r$ permutes the frequencies. Telescope the difference as

$$
\Lambda(a,a,a)-\Lambda(u,u,u)=\Lambda(f,a,a)+\Lambda(u,f,a)+\Lambda(u,u,f).
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the displayed [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) bound each term by $\delta N\max_r|\widehat f(r)|$. Indeed, $\|a\|_2^2=\delta N$ and $\|u\|_2^2=\delta^2N$, so every product of the two remaining [L2 norms](../../../../../../l2-norm.md) is at most $\delta N$. Hence

$$
\max_r|\widehat f(r)|\geq\frac{\delta^2N}{12}.
$$

The zero coefficient vanishes because $\sum f=0$, so choose a nonzero frequency $\theta=r/M$ giving this bound.

Let $Q=\lfloor\sqrt N\rfloor$. The [pigeonhole principle](../../../../../../pigeonhole-principle.md) applied to the $Q+1$ fractional parts $0,\theta,\ldots,Q\theta$ in $Q$ intervals gives an [integer](../../../../../../integer.md) $1\leq q\leq Q$ with $\|q\theta\|_{\mathbb R/\mathbb Z}\leq1/Q$. Partition each [residue class](../../../../../../residue-class.md) modulo $q$ in $[N]$ into consecutive [arithmetic progressions](../../../../../../arithmetic-progression.md) of exactly

$$
L=\left\lfloor\frac{\delta^2\sqrt N}{1000}\right\rfloor
$$

elements, leaving fewer than $L$ remainder points per residue. The total remainder $R_0$ has size at most $qL\leq\delta^2N/1000$. The size hypothesis gives $L\geq\delta^2\sqrt N/2000$. On a full [arithmetic progression](../../../../../../arithmetic-progression.md) $P$, the phase $e^{-2\pi i\theta x}$ varies from its value at the first point by at most $2\pi L/Q\leq4\pi\delta^2/1000$.

Let $F_P=\sum_{x\in P}f(x)$. Replacing the phase by its first value on each full [arithmetic progression](../../../../../../arithmetic-progression.md) and estimating the remainder using $|f|\leq1$ gives

$$
\sum_P|F_P|\geq\frac{\delta^2N}{12}-\frac{(4\pi+1)\delta^2N}{1000}>\frac{\delta^2N}{16}.
$$

Also $|\sum_PF_P|=|\sum_{R_0}f|\leq\delta^2N/1000$. Therefore the sum of the positive $F_P$ is

$$
\frac12\left(\sum_P|F_P|+\sum_PF_P\right)>\frac{\delta^2N}{64}.
$$

Since the total length of these [arithmetic progressions](../../../../../../arithmetic-progression.md) is at most $N$, at least one has $F_P/|P|\geq\delta^2/64$. Thus the step just proved is

$$
\boxed{|P|\geq\frac{\delta^2\sqrt N}{2000},\qquad\frac{|A\cap P|}{|P|}\geq\delta+\frac{\delta^2}{64}.}
$$

An [affine map](../../../../../../affine-map.md) taking this [arithmetic progression](../../../../../../arithmetic-progression.md) to $[|P|]$ preserves the absence of nonconstant three-term [arithmetic progressions](../../../../../../arithmetic-progression.md).

Now iterate. Write $N_j,\delta_j$ for successive lengths and [subset densities](../../../../../../density-of-a-finite-subset.md), with $N_0=N$ and $\delta_0=\delta$. Since every [subset density](../../../../../../density-of-a-finite-subset.md) is at most one,

$$
\frac1{\delta_{j+1}}\leq\frac1{\delta_j}-\frac1{64+\delta_j}\leq\frac1{\delta_j}-\frac1{65}.
$$

Consequently $T=\lceil65/\delta\rceil$ successful steps are impossible. On the other hand, [subset densities](../../../../../../density-of-a-finite-subset.md) never decrease, so with $B=\log(2000/\delta^2)$,

$$
\log N_{j+1}\geq\frac12\log N_j-B,\qquad\log N_j\geq2^{-j}\log N-2B.
$$

Suppose $\delta\log\log N>100$. Since $T\leq66/\delta$,

$$
2^{-T}\log N>\exp\left(\frac{100-66\log2}{\delta}\right)>e^{54/\delta}.
$$

Let $D=\log(4\cdot10^6\delta^{-4})$. We have $2B+D<31+8\log(1/\delta)\leq39/\delta<e^{54/\delta}$. Therefore every length through step $T$ satisfies $\log N_j>D$, and hence $N_j\geq4\cdot10^6\delta^{-4}\geq4\cdot10^6\delta_j^{-4}$. The [density increment](../../../../../../density-increment.md) lemma remains applicable for all $T$ steps, contradicting the reciprocal-density bound.

Thus $\delta\log\log N\leq100$, proving the boxed theorem. The proof includes the [Fourier analysis on a finite abelian group](../../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md) detection, conversion to an [integer](../../../../../../integer.md) [arithmetic progression](../../../../../../arithmetic-progression.md), and the length bookkeeping that produces the double logarithm.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
