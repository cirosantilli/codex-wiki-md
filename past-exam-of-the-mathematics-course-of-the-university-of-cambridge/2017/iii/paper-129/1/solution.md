<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the usual convention that a three-term [arithmetic progression](../../../../../arithmetic-progression.md) must be nonconstant. **There is a genuine small-case defect in the printed statement:** for $n=1$, $\delta=1$, and $A=\{1\}$, neither conclusion can hold with $c_2>0$. We prove the intended [Roth density-increment step](../../../../../roth-density-increment-step.md) for every [odd integer](../../../../../odd-integer.md) $n\geq3$, including the small values of $n$, rather than silently treating $n=1$ as covered. Counting constant [arithmetic progressions](../../../../../arithmetic-progression.md) would make the first alternative vacuous for every nonempty $A$.

Suppose that $A$ has no nonconstant three-term [arithmetic progression](../../../../../arithmetic-progression.md), and let $\alpha=|A|/n$ be its actual [density of a finite subset](../../../../../density-of-a-finite-subset.md). Thus $0<\delta\leq\alpha\leq1$. Put $I=[n]$, $N=2n+1$, and embed $I$ in the [cyclic group](../../../../../cyclic-group.md) $G=\mathbb Z/N\mathbb Z$. A congruence $x-2y+z=0\pmod N$ with $x,y,z\in I$ is an equality over the [integers](../../../../../integer.md), since $|x-2y+z|\leq2(n-1)<N$. Thus this embedding creates no extra three-term [arithmetic progressions](../../../../../arithmetic-progression.md). Since $N$ is odd, multiplication by two permutes $G$.

Use [normalized Fourier analysis on a finite abelian group](../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md), with $e_N(t)=\exp(2\pi it/N)$ and $\widehat h(r)=\mathbb E_{x\in G}h(x)e_N(-rx)$. For the normalized trilinear [arithmetic progression](../../../../../arithmetic-progression.md) count, [character orthogonality](../../../../../character-orthogonality.md) gives

$$
\Lambda(h_1,h_2,h_3)=\mathbb E_{x,d\in G}h_1(x)h_2(x+d)h_3(x+2d)
=\sum_{r\in G}\widehat h_1(r)\widehat h_2(-2r)\widehat h_3(r).
$$

Indeed, expanding each [function](../../../../../function-split.md) in its inverse [Fourier transform](../../../../../fourier-transform.md), averaging in $d$ forces $r_2+2r_3=0$, and averaging in $x$ then forces $r_1=r_3$. The [Parseval identity](../../../../../parseval-identity.md) in this normalization is $\sum_r|\widehat h(r)|^2=\mathbb E_x|h(x)|^2$.

Let $a=1_A$, $b=\alpha1_I$, and $f=a-b$, the [balanced indicator function of a finite subset](../../../../../balanced-indicator-function-of-a-finite-subset.md). Then $\widehat f(0)=0$. Only constant [arithmetic progressions](../../../../../arithmetic-progression.md) contribute to $\Lambda(a,a,a)$, whereas summing $2\min(y-1,n-y)+1$ over centers $y\in I$ counts $(n^2+1)/2$ ordered three-term [arithmetic progressions](../../../../../arithmetic-progression.md) in $I$. Hence

$$
\Lambda(a,a,a)=\frac{\alpha n}{N^2},\qquad
\Lambda(b,b,b)=\frac{\alpha^3(n^2+1)}{2N^2}.
$$

Set $M=\max_r|\widehat f(r)|$. Telescope by changing one factor at a time:

$$
\Lambda(a,a,a)-\Lambda(b,b,b)
=\Lambda(f,a,a)+\Lambda(b,f,a)+\Lambda(b,b,f).
$$

In the [Fourier transform](../../../../../fourier-transform.md) formula for each term, bound the [Fourier coefficient](../../../../../fourier-coefficient.md) of $f$ by $M$ and apply the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) to the other two factors. The permutation $r\mapsto-2r$ preserves the required squared sums. Since $\|a\|_2^2=\alpha n/N$ and $\|b\|_2^2=\alpha^2n/N$, this gives

$$
|\Lambda(a,a,a)-\Lambda(b,b,b)|
\leq M\frac nN(\alpha+\alpha^{3/2}+\alpha^2)
\leq3M\frac{\alpha n}{N}.
$$

If $n\geq4\delta^{-2}$, then $\alpha^2n\geq4$, so the difference in the other direction is at least $\alpha^3n^2/(4N^2)$. Consequently [Fourier detection of a progression-free subset of an interval](../../../../../fourier-detection-of-a-progression-free-subset-of-an-interval.md) gives a nonzero frequency $r$ with

$$
|\widehat f(r)|\geq\frac{\alpha^2n}{12N}\geq\frac{\alpha^2}{36}\geq\frac{\delta^2}{36}.
$$

To turn this into a [density increment](../../../../../density-increment.md), take $Q=\lfloor\sqrt n\rfloor$. The [Dirichlet approximation theorem](../../../../../dirichlet-s-approximation-theorem.md), proved here by placing $0,r/N,\ldots,Qr/N$ into $Q$ equal intervals modulo one, gives $1\leq q\leq Q$ such that $\|qr/N\|_{\mathbb R/\mathbb Z}\leq1/Q$. Define

$$
N_0(\delta)=\left\lceil\max\left\{9,4\delta^{-2},(1152\pi\delta^{-2})^2\right\}\right\rceil,
\qquad L=\left\lfloor\frac{\delta^2Q}{288\pi}\right\rfloor.
$$

For $n\geq N_0(\delta)$, the inequalities $Q\geq\sqrt n/2$ and $\delta^2Q/(288\pi)\geq2$ show that

$$
\frac{\delta^2\sqrt n}{1152\pi}\leq L,\qquad 2L\leq Q.
$$

Use a [progression partition with nearly constant linear phase](../../../../../progression-partition-with-nearly-constant-linear-phase.md): every residue chain of $I$ modulo $q$ has at least $\lfloor n/q\rfloor\geq Q$ points. Split each chain into blocks of $L$ consecutive chain points, merging any remainder into its last full block. This partitions $I$ into [arithmetic progressions](../../../../../arithmetic-progression.md) $P$ with $L\leq|P|<2L$ and common difference $q$.

On a block $P$ with first point $z_P$, the [linear phase](../../../../../linear-phase.md) $\chi(x)=e_N(-rx)$ satisfies

$$
|\chi(x)-\chi(z_P)|\leq\frac{4\pi L}{Q}\leq\frac{\delta^2}{72}.
$$

Let $S_P=\sum_{x\in P}f(x)=|A\cap P|-\alpha|P|$. Freezing the [linear phase](../../../../../linear-phase.md) on each block introduces error at most $(\delta^2/72)N^{-1}\sum_{x\in I}|f(x)|\leq\delta^2/72$. Therefore

$$
\frac1N\sum_P|S_P|\geq
\left|\frac1N\sum_P\chi(z_P)S_P\right|
\geq|\widehat f(r)|-\frac{\delta^2}{72}
\geq\frac{\delta^2}{72}.
$$

The block sums total zero. Their positive part consequently totals at least $N\delta^2/144$. Since all block lengths total $n$, some block has $S_P/|P|\geq N\delta^2/(144n)\geq\delta^2/72$. Its [density of a finite subset](../../../../../density-of-a-finite-subset.md) is at least $\alpha+\delta^2/72\geq\delta(1+\delta/72)$.

For the remaining $3\leq n<N_0(\delta)$, divide $I$ into disjoint consecutive triples and a remainder of at most two points. A three-term-[arithmetic progression](../../../../../arithmetic-progression.md)-free $A$ uses at most two points of each triple, so $\alpha\leq4/5$; the largest ratio occurs at $n=5$. Any [singleton set](../../../../../singleton-mathematics.md) from $A$ then has [density of a finite subset](../../../../../density-of-a-finite-subset.md) one, which is at least $\delta+\delta^2/72$. We may therefore use the explicit constants

$$
\boxed{c_2=\frac1{72},\qquad
c_1(\delta)=\min\left\{\frac{\delta^2}{1152\pi},\frac1{\sqrt{N_0(\delta)}}\right\}.}
$$

In the large case the constructed [arithmetic progression](../../../../../arithmetic-progression.md) has length at least $c_1\sqrt n$; in the small case its length one does too. Thus these constants prove the intended result for all [odd integers](../../../../../odd-integer.md) $n\geq3$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 129](../../paper-129-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
