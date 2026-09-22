<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We give a quantitative construction for the whole open set, including the case of infinitely many component intervals. Pointwise divergence at a single point is insufficient here. Write $z=e^{2\pi it}$ and use normalized measure on $\mathbb T$.

First let $K$ be a finite union of closed arcs with $|K|\le3\varepsilon$, where $\varepsilon$ is small. Choose a [smooth function](../../../../../../smooth-function.md) nonnegative [function](../../../../../../function-split.md) $u$, equal to one on $K$, with $u\le1$ and $\eta:=\int u\le6\varepsilon$. This follows by making the transition regions around the finitely many arc endpoints sufficiently short. Define the analytic [Herglotz integral](../../../../../../schwarz-integral-on-the-unit-disk.md)

$$
G(z)=\frac{\eta+\displaystyle\int_{\mathbb T}\frac{e^{2\pi is}+z}{e^{2\pi is}-z}u(s)\,ds}{2\eta}.
$$

Its real part is $(\eta+P[u](z))/(2\eta)>0$, where $P[u]$ is the [disk Poisson integral](../../../../../../poisson-integral-on-the-unit-disk.md), and $G(0)=1$. Smoothness of $u$ makes $G$ [continuous](../../../../../../continuous-function.md) and [smooth function](../../../../../../smooth-function.md) up to the circle; on $K$ its boundary real part is at least $1/(2\eta)$. The branch $H=\log G$ therefore has $H(0)=0$ and

$$
|\operatorname{Im}H|<\pi/2,\qquad
\operatorname{Re}H\ge\log\frac1{12\varepsilon}\quad\text{on }K.
$$

The [complex logarithm](../../../../../../complex-logarithm.md) has no branch problem because $G$ lies in the right half-plane. Its [smooth function](../../../../../../smooth-function.md) boundary values give absolutely summable Taylor coefficients. Choose an analytic [polynomial](../../../../../../polynomial-split.md) $A$, with zero constant coefficient, uniformly within $1/4$ of $H$ on the closed disk. Put $P(t)=\operatorname{Im}A(e^{2\pi it})/\pi$. Then $\|P\|_\infty\le1/2+1/(4\pi)<1$.

If $D=\deg A$ and $m>D$, the modulated [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) $Q(t)=e^{2\pi imt}P(t)$ has spectrum in $[m-D,m+D]$. A sharp [Fourier partial sum](../../../../../../fourier-partial-sum.md) at $m$ selects exactly the negative-frequency half of $P$, since $A(0)=0$:

$$
S_m(Q,t)=-\frac{e^{2\pi imt}\overline{A(e^{2\pi it})}}{2\pi i}.
$$

Consequently, for every $t\in K$,

$$
|S_m(Q,t)|\ge B(\varepsilon):=\frac{\log(1/(12\varepsilon))-1/4}{2\pi},\qquad\|Q\|_\infty\le1.
$$

**The carrier frequency $m$ can be arbitrarily large.** This [compact-set Fourier amplification lemma](../../../../../../compact-set-fourier-amplification-lemma.md) uses a bounded imaginary part to obtain a large one-sided [Fourier multiplier](../../../../../../fourier-multiplier.md); no assertion about pointwise divergence is used.

Now let $E$ be any open set of measure $\delta$. Define

$$
\psi(\delta)=\max\{0,B(\delta)/4-1\}.
$$

If this is zero take $f=0$. Otherwise choose a decreasing sequence $\delta_j\downarrow0$, with $\delta_1=\delta$, so small for $j\ge2$ that

$$
2^{-j}B(\delta_j)\ge\psi(\delta)+2.
$$

For $j=1$ this inequality also holds: $B(\delta)>4$ and $B(\delta)/2\ge B(\delta)/4+1$. Let $L_j$ be an increasing compact exhaustion of $E$.

Using [compact batching of a small open set](../../../../../../compact-batching-of-a-small-open-set.md), we recursively choose finite closed-arc unions $K_j\subset E$, of measure at most $3\delta_j$, such that $L_j$ is covered by the interiors of $K_1,\ldots,K_j$ and

$$
\left|E\setminus\operatorname{int}(K_1\cup\cdots\cup K_j)\right|\le\delta_{j+1}.
$$

Here is the measure-theoretic justification. At step $j$, the uncovered portion has measure at most $\delta_j$. Its intersection with $L_j$ after removing the previously covered interiors is compact, and can be covered by finitely many closed arcs lying in $E$ with total length at most $\delta_j$ plus an arbitrarily small excess. By [inner regularity of Lebesgue measure](../../../../../../inner-regularity-of-lebesgue-measure.md), a further compact subset of the uncovered open portion captures all but $\delta_{j+1}$ of its measure; cover it similarly. The combined finite arc union has length at most $3\delta_j$. This both covers the outstanding part of $L_j$ and ensures the next remainder estimate. In particular $E\subset\bigcup_jK_j$.

Apply the finite-arc construction to $K_j$ to get $P_j$ of degree $D_j$. Choose carriers $m_j$ recursively so that the bands $[m_j-D_j,m_j+D_j]$ are positive and strictly ordered with no overlap. Set

$$
f(t)=\sum_{j=1}^\infty2^{-j}e^{2\pi im_jt}P_j(t).
$$

The [frequency-separated Fourier block series](../../../../../../frequency-separated-fourier-block-series.md) and the [Weierstrass M-test](../../../../../../weierstrass-m-test.md) give a [continuous](../../../../../../continuous-function.md) complex-valued [function](../../../../../../function-split.md) with $\|f\|_\infty\le\sum_j2^{-j}=1$. At the cutoff $m_j$, all earlier bands have been included in full and every later band is absent. Thus on $K_j$,

$$
|S_{m_j}(f,t)|\ge2^{-j}B(\delta_j)-\left|\sum_{i<j}2^{-i}e^{2\pi im_it}P_i(t)\right|
\ge\psi(\delta)+2-1>\psi(\delta).
$$

Every point of $E$ lies in some $K_j$, so

$$
\boxed{S^*(f,t)\ge\psi(\delta)\quad(t\in E),\qquad
\psi(\delta)\sim\frac1{8\pi}\log\frac1\delta\longrightarrow\infty.}
$$

Values of $\psi$ outside $0<\delta\le1$ may be defined arbitrarily. The construction handles an arbitrary open set, not just one point or a finite collection of intervals. It also prevents cancellation explicitly: earlier bands contribute a bounded complete sum, and later bands contribute nothing at the chosen cutoff.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [Section A](../../section-a.md)
4. [Paper 82](../../../paper-82-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
