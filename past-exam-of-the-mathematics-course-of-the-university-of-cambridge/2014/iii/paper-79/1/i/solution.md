<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Roth theorem on three-term arithmetic progressions](../../../../../../roth-theorem-on-three-term-arithmetic-progressions.md) says that, for each fixed $\delta>0$, a sufficiently long interval cannot have a subset of [density of a finite subset](../../../../../../density-of-a-finite-subset.md) at least $\delta$ with no nonconstant three-term [arithmetic progression](../../../../../../arithmetic-progression.md). Equivalently, the maximum size of a three-term-progression-free subset of $[N]=\{1,\ldots,N\}$ is $o(N)$. Here is a [density increment](../../../../../../density-increment.md) proof, including its analytic ingredients.

Write $e(t)=\exp(2\pi it)$ and embed $I=[N]$ into the [cyclic group](../../../../../../cyclic-group.md) $G=\mathbb Z/(2N+1)\mathbb Z$ of order $M$. For [normalized Fourier analysis on a finite abelian group](../../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md) take $\widehat h(r)=M^{-1}\sum_xh(x)e(-rx/M)$. The [orthogonality of complex exponentials](../../../../../../orthogonality-of-complex-exponentials.md) follows from a [finite geometric series](../../../../../../finite-geometric-series.md): its average is zero for a nonzero frequency and one for frequency zero. Expanding in these [linear phases](../../../../../../linear-phase.md) consequently proves both [Fourier inversion on a finite group](../../../../../../fourier-inversion-on-a-finite-group.md) and the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md). In particular,

$$
\mathbb E_x|h(x)|^2=\sum_r|\widehat h(r)|^2,
\qquad
\Lambda(h_0,h_1,h_2):=\mathbb E_{x,d}h_0(x)h_1(x+d)h_2(x+2d)
=\sum_r\widehat h_0(r)\widehat h_1(-2r)\widehat h_2(r).
$$

The second identity follows by summing the frequency expansion over $x,d$: the two constraints leave precisely the frequencies $(r,-2r,r)$. Since $M$ is odd, multiplication by two permutes the frequencies. Also a congruence $x+z=2y$ with $x,y,z\in I$ is an equality in the [integers](../../../../../../integer.md), since $|x+z-2y|<M$.

Let $A\subseteq I$ have [subset density](../../../../../../density-of-a-finite-subset.md) $\alpha=|A|/N\geq\delta$, and suppose it contains no nonconstant three-term [arithmetic progression](../../../../../../arithmetic-progression.md). Its [balanced indicator function of a finite subset](../../../../../../balanced-indicator-function-of-a-finite-subset.md) is $f=1_A-\alpha1_I$, extended by zero outside $I$. Then $\widehat f(0)=0$. Counting endpoints with the same parity gives

$$
\Lambda(1_A,1_A,1_A)=\frac{\alpha N}{M^2},
\qquad
\Lambda(\alpha1_I,\alpha1_I,\alpha1_I)
=\frac{\alpha^3\lceil N^2/2\rceil}{M^2}.
$$

If $N\geq4\alpha^{-2}$, their difference in absolute value is at least $\alpha^3N^2/(4M^2)$. Telescope the difference of the products into three terms, each containing $f$ and two factors chosen from $1_A,\alpha1_I$. Put $s=\max_r|\widehat f(r)|$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) bound each term by $s\alpha N/M$, since the squared normalized $L^2$ norm of either other factor is at most $\alpha N/M$. Therefore some nonzero frequency $r$ satisfies

$$
 s\geq\frac{\alpha^2N}{12M}\geq\frac{\alpha^2}{36},
 \qquad
 \left|\sum_{x\in I}f(x)e(-rx/M)\right|\geq\frac{\alpha^2N}{36}.
$$

This is the [Fourier detection of a progression-free subset of an interval](../../../../../../fourier-detection-of-a-progression-free-subset-of-an-interval.md) step; it has just been proved rather than assumed.

We now turn this [Fourier coefficient on a finite abelian group](../../../../../../fourier-coefficient-on-a-finite-abelian-group.md) into a [density increment](../../../../../../density-increment.md). Set $Q=\lfloor\sqrt N\rfloor$. Partition the unit interval into $Q$ equal pieces and place the $Q+1$ [fractional parts](../../../../../../fractional-part.md) of $0,r/M,\ldots,Qr/M$ in them. The [pigeonhole principle](../../../../../../pigeonhole-principle.md) gives $1\leq q\leq Q$ with $\|qr/M\|\leq1/Q$. This proves the particular [Dirichlet approximation theorem](../../../../../../dirichlet-s-approximation-theorem.md) needed here. Put $\kappa=\alpha^2/(1000\pi)$ and $L=\lfloor\kappa Q\rfloor$. For sufficiently large $N$ depending only on $\delta$, $L\geq\kappa Q/2$ and $2L\leq Q$. Each residue chain modulo $q$ in $I$ has at least $Q$ elements. Split each such chain into [arithmetic progressions](../../../../../../arithmetic-progression.md) with between $L$ and $2L-1$ elements, absorbing its final short remainder into the previous block.

The [linear phase](../../../../../../linear-phase.md) changes by at most $4\pi L/Q\leq\alpha^2/250$ within any block. Freezing the [linear phase](../../../../../../linear-phase.md) at the first element of each block therefore changes the preceding correlation by at most $\alpha^2N/250$, because $|f|\leq1$. The [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\sum_P\left|\sum_{x\in P}f(x)\right|\geq\frac{\alpha^2N}{72}.
$$

The block sums of the [balanced indicator function of a finite subset](../../../../../../balanced-indicator-function-of-a-finite-subset.md) add to zero, so their positive total is half their absolute total. Some block consequently satisfies

$$
\boxed{\quad |P|\geq c\alpha^2\sqrt N,\qquad
\frac{|A\cap P|}{|P|}\geq\alpha+\frac{\alpha^2}{144}.\quad}
$$

Here $c>0$ is absolute, and shrinking it absorbs the floors. An affine parametrization of $P$ identifies $A\cap P$ with a subset of $[|P|]$ and preserves [arithmetic progressions](../../../../../../arithmetic-progression.md).

Repeat this [Roth density-increment step](../../../../../../roth-density-increment-step.md). Every step raises the [subset density](../../../../../../density-of-a-finite-subset.md) by at least $\delta^2/144$, so fewer than $T=\lceil144/\delta^2\rceil+1$ steps are possible. All the lengths satisfy $N_{j+1}\geq c\delta^2\sqrt{N_j}$ while above a threshold depending only on $\delta$. Choose the initial $N$ so large that this lower recursion stays above that threshold for $T$ steps; this is possible by working backwards through finitely many squarings. We would then force a [subset density](../../../../../../density-of-a-finite-subset.md) greater than one. **Thus every fixed positive density eventually forces a nonconstant three-term arithmetic progression.** For an infinite subset of the positive [integers](../../../../../../integer.md) with positive [upper asymptotic density](../../../../../../upper-asymptotic-density.md), apply the finite conclusion along initial intervals whose [subset density](../../../../../../density-of-a-finite-subset.md) is bounded away from zero; this gives the usual infinite formulation as well.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
