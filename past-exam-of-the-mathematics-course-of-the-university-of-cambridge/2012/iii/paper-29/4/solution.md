<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A precise useful form of the principle is the [type I–type II inverse principle for Möbius correlation](../../../../../type-i-type-ii-inverse-principle-for-mobius-correlation.md). Normalize $|f(n)|\leq1$, and suppose

$$
\left|\sum_{n\leq X}\mu(n)f(n)\right|\geq\delta X.
$$

For any positive integer cutoffs $U,V$ with $U+V\leq\delta X/2$, define

$$
c_d=\sum_{\substack{bc=d\\b\leq U,\ c\leq V}}\mu(b)\mu(c),
\qquad a_d=\sum_{\substack{c\mid d\\c>V}}\mu(c).
$$

Then $|c_d|,|a_d|\leq\tau(d)$, where $\tau$ is the [divisor function](../../../../../divisor-function.md), and at least one of the following two sums has modulus at least $\delta X/4$:

$$
T_{\mathrm I}=\sum_{d\leq UV}c_d\sum_{k\leq X/d}f(dk),
\qquad
T_{\mathrm {II}}=\sum_{\substack{d>V,\ w>U\\dw\leq X}}a_d\mu(w)f(dw).
$$

The first is correlation against a controlled linear combination of indicators of multiples of small moduli, each a [periodic function](../../../../../periodic-function.md): this is the “somewhat periodic” branch. The second is a [bilinear sum](../../../../../bilinear-sum.md) with independently weighted factors, both larger than the cutoffs: this is the “somewhat multiplicative” branch. The statement concerns these precise correlations, not an assertion that $f$ must itself be periodic or multiplicative.

For clarity, the [Vaughan identity for the Möbius function](../../../../../vaughan-identity-for-the-mobius-function.md) proves this version immediately. Split $\mu=\mu_{\leq U}+\mu_{>U}$ and likewise at $V$. Since $\mu*\mu*\mathbf1=\mu$,

$$
\boxed{\mu=\mu_{\leq U}+\mu_{\leq V}
-\mu_{\leq U}*\mu_{\leq V}*\mathbf1
+\mu_{>U}*\mu_{>V}*\mathbf1.}
$$

Multiply by $f(n)$ and sum. The first two terms contribute at most $U+V$ in modulus, and the remaining terms are $-T_{\mathrm I}+T_{\mathrm {II}}$. The [triangle inequality](../../../../../triangle-inequality.md) gives the stated dichotomy. It is valid at finite $X$ and for any chosen cutoffs in the indicated range.

We now prove the required orthogonality without appealing to a stronger uniform exponential-sum theorem. Write $\alpha=\sqrt2$ and $e(u)=e^{2\pi iu}$. The [Diophantine bound for the square root of two](../../../../../diophantine-bound-for-the-square-root-of-two.md) is

$$
\|h\alpha\|\geq\frac1{4h}\qquad(h\geq1),
$$

where $\|u\|$ is distance to the nearest integer. If $a$ is that nearest integer, then $|2h^2-a^2|\geq1$, while $h\sqrt2+a\leq4h$; dividing proves the bound.

Use the preceding [Dirichlet convolution](../../../../../dirichlet-convolution.md) identity with $U=V=P=\lfloor X^{1/10}\rfloor$. The two short terms are $O(P)$. For the [type I sum](../../../../../type-i-sum.md), the [exponential geometric sum bound](../../../../../exponential-geometric-sum-bound.md) gives

$$
\left|\sum_{k\leq X/d}e(\alpha dk)\right|
\ll\min\{X/d,\|d\alpha\|^{-1}\}\ll d.
$$

Consequently

$$
|T_{\mathrm I}|\ll\sum_{d\leq P^2}\tau(d)d
\ll P^4\log(2P)=O(X^{2/5}\log X),
$$

using $\sum_{d\leq Y}\tau(d)\ll Y\log(2Y)$ from counting factor pairs.

For the [type II sum](../../../../../type-ii-sum.md), perform a [dyadic decomposition](../../../../../dyadic-decomposition.md) into $d\in(D,2D]$, $w\in(W,2W]$, keeping $dw\leq X$. Nonempty blocks have $DW<X$, while $D,W\gg P$. A block $B$ satisfies, by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and the [divisor-square summatory bound](../../../../../divisor-square-summatory-bound.md),

$$
|B|^2\ll D\log^3X\left(DW+W\sum_{1\leq h\leq W}\min\{D,\|h\alpha\|^{-1}\}\right).
$$

To justify the cutoff, after expanding the square the permissible $d$ for a pair $w,w'$ still form an interval, with upper endpoint $\min(2D,X/\max(w,w'))$. Its exponential sum has the same geometric bound. Diagonal pairs supply $DW$; for each nonzero difference $h=w-w'$ there are $O(W)$ pairs.

The points $0,\alpha,2\alpha,\ldots,\lfloor W\rfloor\alpha$ modulo one are separated by at least $1/(4W)$. Counting points in consecutive distance bands around zero therefore gives

$$
\sum_{1\leq h\leq W}\|h\alpha\|^{-1}\ll W\log(2W).
$$

Substitution yields the [bilinear cancellation for badly approximable phases](../../../../../bilinear-cancellation-for-badly-approximable-phases.md) estimate

$$
|B|\ll DW\log^2X\left(D^{-1/2}+W^{-1/2}\right)
\ll X\log^2X\,P^{-1/2}.
$$

There are $O(\log^2X)$ blocks, so $T_{\mathrm {II}}\ll X^{19/20}\log^4X$. The divisor-square bound itself can be obtained elementarily from $\tau(n)^2\leq\tau_4(n)$ prime-power by prime-power and $\sum_{n\leq Y}\tau_4(n)\leq Y(1+\log Y)^3$; no uncontrolled coefficient bound is being suppressed.

Combining the short, type I and type II terms,

$$
\left|\sum_{n\leq X}\mu(n)e(n\sqrt2)\right|
\ll X^{2/5}\log X+X^{19/20}\log^4X+X^{1/10}=o(X).
$$

Hence

$$
\boxed{\lim_{X\to\infty}\frac1X\left|\sum_{n\leq X}\mu(n)e(n\sqrt2)\right|=0.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
