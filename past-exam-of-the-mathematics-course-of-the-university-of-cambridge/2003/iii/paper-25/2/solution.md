<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We prove the three-term [Roth theorem](../../../../../roth-s-theorem.md) by a [density increment](../../../../../density-increment.md), keeping the interval boundary rather than replacing the interval by a cyclic group with a different density. The case $\delta>1$ is vacuous; assume $0<\delta\le1$.

We first prove the following alternative with absolute constants $c,C>0$: if $A\subseteq[1,N]$ has density $\eta$ and no nonconstant three-term [arithmetic progression](../../../../../arithmetic-progression.md), and $N\ge C\eta^{-4}$, then some integer progression $P\subseteq[1,N]$ has

$$
|P|\ge c\eta^2\sqrt N,\qquad |A\cap P|/|P|\ge\eta+c\eta^2.
$$

For this purpose take $M=6\lceil4N/6\rceil+1$, so $4N<M\le5N$ for large $N$ and $2,3$ are invertible modulo $M$. On $G=\mathbb Z/M\mathbb Z$, put $I=1_{[1,N]}$, $a=1_A$, $g=\eta I$ and $f=a-g$. In particular $\sum f=0$, and $f$ vanishes outside the interval. Use normalized [Fourier coefficients on a finite abelian group](../../../../../fourier-coefficient-on-a-finite-abelian-group.md), $\widehat u(r)=M^{-1}\sum_xu(x)e(-rx/M)$. Character orthogonality, obtained by summing a finite geometric series, gives [Fourier inversion on a finite group](../../../../../fourier-inversion-on-a-finite-group.md) and [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md).

For $\Lambda(u,v,w)=\mathbb E_{x,d}u(x)v(x+d)w(x+2d)$ these identities give

$$
\Lambda(u,v,w)=\sum_r\widehat u(r)\widehat v(-2r)\widehat w(r).
$$

There is no wrapping ambiguity when all three entries lie in $[1,N]$: the integer $x-2y+z$ has absolute value below $M$, so a modular relation is an integer relation. If no nonconstant progression exists, $\Lambda(a,a,a)=|A|/M^2$. Meanwhile the choices $1\le x\le\lfloor N/4\rfloor$ and $1\le d\le\lfloor N/8\rfloor$ give $\Lambda(I,I,I)\ge1/10000$ for sufficiently large $N$.

Expand the difference by telescoping,

$$
\Lambda(a,a,a)-\Lambda(g,g,g)
=\Lambda(f,a,a)+\Lambda(g,f,a)+\Lambda(g,g,f).
$$

If $\rho=\max_r|\widehat f(r)|$, each term on the right has modulus at most $\rho\eta N/M$. Indeed multiplication of frequencies by $2$ permutes them, and [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) with [Parseval identity](../../../../../parseval-identity.md) bounds the two other Fourier factors by their $L^2$ norms; each squared norm is at most $\eta N/M$. For $N\ge10000\eta^{-2}$, the diagonal count is less than half the main density term. Therefore

$$
3\rho\eta N/M\ge\eta^3/20000.
$$

In particular there is a nonzero frequency $r$ with

$$
\left|\sum_{x=1}^N f(x)e(-rx/M)\right|\ge\gamma N,
\qquad \gamma=\eta^2/20000.
$$

The frequency is nonzero because $\widehat f(0)=0$.

Here is the conversion of this coefficient into a density increment. Put $Q=\lfloor\sqrt N\rfloor$. Of the $Q+1$ numbers $0,\theta,\ldots,Q\theta$ modulo one, two lie in the same one of $Q$ equal arcs. Their difference gives $1\le q\le Q$ with $\|q\theta\|\le1/Q$, where $\theta=-r/M$. This is the needed [Dirichlet approximation theorem](../../../../../dirichlet-s-approximation-theorem.md), proved by the [pigeonhole principle](../../../../../pigeonhole-principle.md).

Partition each residue class modulo $q$ in $[1,N]$ into consecutive progressions of length $L=\lfloor\gamma Q/(100\pi)\rfloor$, leaving its final short tail. Their total tail size is at most $qL\le\gamma N/(100\pi)$. On each full progression the character differs from its value at the first point by at most $2\pi L/Q\le\gamma/50$. Hence removing tails and replacing the character by its initial value shows

$$
\sum_{P\text{ full}}\left|\sum_{x\in P}f(x)\right|\ge\tfrac12\gamma N.
$$

The sum of $f$ over all full progressions is the negative of its sum over the tails, so its absolute value is at most $\gamma N/(100\pi)$. Consequently the sum of the positive block sums is at least $\gamma N/5$. Since these blocks contain at most $N$ points in total, at least one has average $f$ at least $\gamma/5$. It gives a density increment at least $\eta^2/100000$. For $N\ge C\eta^{-4}$ with a sufficiently large absolute $C$, $L\ge c\eta^2\sqrt N$. This proves the alternative, with one small common absolute $c$.

Reidentify $P$ with $[1,|P|]$ by its affine parametrization. Absence of a nonconstant progression is preserved, while density increases. At every step the density is at least the original $\delta$, so the increment is at least $c\delta^2$ and the new interval length is at least $c\delta^2\sqrt{N_{\mathrm{old}}}$. After at most $T=\lceil1/(c\delta^2)\rceil+1$ steps, the density would exceed one. Choose the original $N$ so large that the length stays above $C\delta^{-4}$ throughout these finitely many steps. Such a choice exists explicitly by working backwards: a required next length $L_0$ is ensured by previous length at least $(L_0/(c\delta^2))^2$. The alternative could then be applied at every step, giving a contradiction. Thus

$$
\boxed{\text{for each }\delta>0\text{, all sufficiently long density-}\delta\text{ intervals contain a nonconstant three-term progression}.}
$$

This is the [Roth density increment on an integer progression](../../../../../roth-density-increment-on-an-integer-progression.md) proof.

For the pattern with offsets $0,1,3$, replace the counting functional by $\mathbb E_{x,d}u(x)v(x+d)w(x+3d)$. Its Fourier expression is

$$
\sum_r\widehat u(2r)\widehat v(-3r)\widehat w(r),
$$

coming from the relation $2x-3y+z=0$. Both multipliers are invertible modulo the chosen $M$, so exactly the same Parseval estimates apply. This relation has no wrap in $[1,N]$, since its magnitude is at most $3N<M$, and the earlier restricted choices of $x,d$ still give a fixed positive density main term. The same increment and iteration find a nonconstant triple $\{a,a+d,a+3d\}$. Negative $d$ is allowed, as requested, and the affine reparametrization used in the iteration preserves this pattern as well.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
