<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the phase-distance convention for a [Bohr set](../../../../../bohr-set.md):

$$
B(R,\epsilon)=\{x\in\mathbb Z/N\mathbb Z:\|rx/N\|_{\mathbb R/\mathbb Z}\leq\epsilon\text{ for every }r\in R\},
$$

where the norm is distance to the nearest integer. This is the [Bohr set in phase-distance convention](../../../../../bohr-set-in-phase-distance-convention.md); the alternative condition $|e(rx/N)-1|\leq\rho$ has a different radius and corresponding constants. Assume $d\geq1$, as $1/d$ requires.

For each residue $x$, form $t_x=(rx/N)_{r\in R}$ in the $d$-dimensional torus. Around these $N$ points place translates of a box of side length $\epsilon$ in each coordinate. For $0<\epsilon\leq1$, their volumes sum to $N\epsilon^d$. If $\epsilon>N^{-1/d}$, two boxes overlap, and their distinct indices differ by a nonzero $q$ with every phase distance less than $\epsilon$. Thus **the [Bohr set](../../../../../bohr-set.md) contains a nonzero element at the stated threshold**. For larger radii the entire group is already present.

Letting the box width decrease to $N^{-1/d}$ and using the finite number of possible nonzero $q$, obtain a nonzero $q$ with $\|rq/N\|\leq N^{-1/d}$ for every $r\in R$. By the [triangle inequality](../../../../../triangle-inequality.md), $jq$ lies in $B(R,\epsilon)$ whenever $0\leq j<\epsilon N^{1/d}$. Since $N$ is prime, these multiples are distinct up to length $N$. Therefore, in the usual radius range $0<\epsilon\leq1/2$, the [arithmetic progression](../../../../../arithmetic-progression.md)

$$
\boxed{0,q,2q,\ldots,(L-1)q,\qquad L=\lceil\epsilon N^{1/d}\rceil}
$$

has the requested length. For literally unrestricted $\epsilon>0$, the correct lower bound is $\min(N,\lceil\epsilon N^{1/d}\rceil)$: a progression of distinct residues cannot exceed $N$. For example, $d=1$, $\epsilon=2$ makes the uncapped printed bound impossible. If $R$ is empty, the [Bohr set](../../../../../bohr-set.md) is the whole group and has a progression of length $N$; the displayed exponent is simply inapplicable.

Now transfer the dense integer set to a larger cyclic group. Choose a prime $8N<p<16N$, using [Bertrand's postulate](../../../../../bertrand-s-postulate.md), and regard $A$ as a subset of $G=\mathbb Z/p\mathbb Z$. Its density $\alpha=|A|/p$ is at least $1/1600$. Normalize [Fourier coefficients on a finite abelian group](../../../../../fourier-coefficient-on-a-finite-abelian-group.md) and [convolution](../../../../../convolution.md) by

$$
\widehat f(r)=\mathbb E_{x\in G}f(x)e(-rx/p),\qquad (f*g)(x)=\mathbb E_yf(y)g(x-y).
$$

The [Fourier inversion](../../../../../fourier-inversion-theorem.md) and [Parseval identity](../../../../../parseval-identity.md) formulas are $f(x)=\sum_r\widehat f(r)e(rx/p)$ and $\sum_r|\widehat f(r)|^2=\mathbb E|f|^2$; [convolution](../../../../../convolution.md) turns into multiplication of [Fourier coefficients on a finite abelian group](../../../../../fourier-coefficient-on-a-finite-abelian-group.md).

For $f=\mathbf1_A$, set $R=\{r:|\widehat f(r)|\geq\alpha^{3/2}/2\}$. Then [Parseval identity](../../../../../parseval-identity.md) bounds

$$
|R|\leq4\alpha^{-2}\leq D:=4\cdot1600^2.
$$

Also, with $\widetilde f(x)=f(-x)$, the nonnegative [convolution](../../../../../convolution.md) $Q=f*f*\widetilde f*\widetilde f$ is supported exactly on the modular set $2A-2A$, and

$$
Q(x)=\sum_r|\widehat f(r)|^4e(rx/p).
$$

The frequencies outside $R$ contribute in absolute value at most $(\alpha^3/4)\sum_r|\widehat f(r)|^2=\alpha^4/4$. For $x\in B(R,1/6)$, the real part of each phase from $R$ is at least $1/2$; moreover $0\in R$ and $|\widehat f(0)|^4=\alpha^4$. Hence $Q(x)\geq\alpha^4/4>0$. We have proved the [cyclic Bogolyubov lemma with explicit phase radius](../../../../../cyclic-bogolyubov-lemma-with-explicit-phase-radius.md):

$$
B(R,1/6)\subseteq 2A-2A,\qquad |R|\leq D.
$$

The previous [Bohr set](../../../../../bohr-set.md) argument gives a modular [arithmetic progression](../../../../../arithmetic-progression.md) of length at least $p^{1/D}/6$. The remaining step is [lifting a short modular progression to an integer progression](../../../../../lifting-a-short-modular-progression-to-an-integer-progression.md). Every one of its elements has a unique integer lift belonging to $2A-2A\subseteq[-2N,2N]$. Successive lifted differences lie in $[-4N,4N]$ and are congruent to the same residue. Since $p>8N$, at most one integer in this difference interval represents that residue, so every successive difference is the same. The lifts form a genuine integer [arithmetic progression](../../../../../arithmetic-progression.md), not merely a modular one.

For sufficiently large $N$, the constants can be absorbed into half the exponent. Thus

$$
\boxed{2A-2A\text{ contains an arithmetic progression of length at least }N^c,\qquad c=\frac1{2D}>0.}
$$

No attempt to optimize this absolute constant is needed.

A counterexample comes from [dense integer sets with only logarithmic-length progressions](../../../../../dense-integer-sets-with-only-logarithmic-length-progressions.md). To show that $A$ itself need not have such a progression, choose a random subset $B\subseteq[1,N]$ by independent inclusion with probability $p_0=0.02$. Its size has mean $0.02N$ and variance at most $0.02N$, so [Chebyshev's inequality](../../../../../chebyshev-inequality.md) shows $\mathbb P(|B|<0.01N)\leq200/N$. There are at most $N^2$ increasing [arithmetic progressions](../../../../../arithmetic-progression.md) of any fixed length $L\geq2$, and each belongs to $B$ with probability $p_0^L$. Taking $L=\lceil4\log N/\log(1/p_0)\rceil$ makes the [union bound](../../../../../boole-s-inequality.md) at most $N^{-2}$. For large $N$, some realization has at least $0.01N$ elements and no length-$L$ [arithmetic progression](../../../../../arithmetic-progression.md). Take a subset of exactly $0.01N$ elements. It retains that avoidance. **Such a set has no progression longer than $O(\log N)$**, and therefore no progression of length $N^c$ for any fixed $c>0$, eventually. Interpret the prescribed exact cardinality on values of $N$ where it is integral, or use its integer part.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
