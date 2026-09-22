<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\eta=|A|/N\geq\theta$, $f=1_A$, and use normalized averages on $\mathbb Z_N$. Write $\widehat f(r)=\mathbb E_xf(x)e^{-2\pi irx/N}$ and define the [normalized convolution on a finite group](../../../../../../normalized-convolution-on-a-finite-group.md) by $(g*h)(x)=\mathbb E_yg(y)h(x-y)$. With $\widetilde f(x)=f(-x)$,

$$
F=f*f*\widetilde f*\widetilde f,\qquad F(x)=\sum_r|\widehat f(r)|^4e^{2\pi irx/N}.
$$

These identities follow by expanding the [convolution](../../../../../../convolution.md) and using [character orthogonality](../../../../../../character-orthogonality.md). Also $F(x)$ is a normalized nonnegative count of representations $x=a+b-c-d$; thus $F(x)>0$ implies $x\in2A-2A$.

Take $R=\{r\ne0:|\widehat f(r)|\geq\eta^{3/2}/\sqrt2\}$. The [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) gives

$$
|R|\leq2\eta^{-2}\leq2\theta^{-2},\qquad\sum_{r\notin R\cup\{0\}}|\widehat f(r)|^4\leq\frac{\eta^3}{2}\sum_r|\widehat f(r)|^2=\frac{\eta^4}{2}.
$$

For $x$ in the [Bohr set in phase-distance convention](../../../../../../bohr-set-in-phase-distance-convention.md) $\mathcal B=\{x:\|rx/N\|_{\mathbb R/\mathbb Z}\leq1/6\text{ for every }r\in R\}$, all large-frequency terms have real part at least half their magnitude. Since $F$ is real,

$$
F(x)\geq\eta^4+\frac12\sum_{r\in R}|\widehat f(r)|^4-\frac{\eta^4}{2}>0.
$$

Thus $\mathcal B\subseteq2A-2A$. This proves the [cyclic Bogolyubov lemma](../../../../../../cyclic-bogolyubov-lemma.md) needed here, rather than citing it.

We now find an [arithmetic progression in a cyclic Bohr set](../../../../../../arithmetic-progression-in-a-cyclic-bohr-set.md). Put $m=|R|$. If $m=0$, the whole group lies in $2A-2A$ and the result is immediate. Otherwise [set](../../../../../../set-split.md) $Q=\lfloor N^{1/(m+1)}\rfloor$. When $Q\geq2$, place the $Q^m+1$ vectors $(jr/N)_{r\in R}$, $0\leq j\leq Q^m$, into the $Q^m$ boxes of side $1/Q$ in the $m$-dimensional unit cube. Two occupy the same box, giving $1\leq q\leq Q^m<N$ with $\|qr/N\|\leq1/Q$ for every $r\in R$. The [arithmetic progression](../../../../../../arithmetic-progression.md)

$$
0,q,2q,\ldots,\lfloor Q/6\rfloor q
$$

lies in $\mathcal B$. Its terms are distinct: the order of $q$ in $\mathbb Z_N$ is $N/\gcd(N,q)\geq N/q\geq N/Q^m\geq Q$, greater than its number of steps. Its length is at least $Q/6\geq N^{1/(m+1)}/12$.

Let $D=\lceil2\theta^{-2}\rceil$. Since $m\leq D$, the exponent $1/(m+1)$ is at least $1/(D+1)$. If $Q=1$, then $N^{1/(m+1)}<2$ and the singleton $\{0\}$ already exceeds the required lower bound. This also covers $N=1$. Therefore one may take

$$
\boxed{a=\frac1{12},\qquad b=\frac1{\lceil2\theta^{-2}\rceil+1}.}
$$

The [arithmetic progression](../../../../../../arithmetic-progression.md) here is a [set](../../../../../../set-split.md) of distinct elements in the [cyclic group](../../../../../../cyclic-group.md); this part does not impose the additional integer nonwrapping condition used in Question 3.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
