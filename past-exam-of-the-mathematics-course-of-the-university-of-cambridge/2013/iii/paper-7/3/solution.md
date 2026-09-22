<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The relevant version of [Wiener covering lemma](../../../../../wiener-covering-lemma.md) is the finite ball selection lemma: from a finite collection of open Euclidean balls one can select pairwise disjoint balls $B_j$ such that the original union is contained in $\bigcup_j3B_j$, where $3B_j$ has the same centre and three times the radius. To prove it, repeatedly retain a largest-radius remaining ball and discard every ball meeting it. If a discarded ball has radius $r\leq R$ and meets a retained ball of radius $R$, every point of the former is at distance less than $r+(r+R)\leq3R$ from the latter's centre. This proves the containment and, by scaling [Lebesgue measure](../../../../../lebesgue-measure.md),

$$
\lambda_d\left(\bigcup\text{ original balls}\right)
\leq3^d\sum_j\lambda_d(B_j).
$$

This is a covering result; no Fourier-algebra version of Wiener's lemma is involved.

We use it for a [disjoint ball decomposition modulo null sets](../../../../../disjoint-ball-decomposition-modulo-null-sets.md) of $V$. The empty set needs only the empty family. Otherwise put $V_0=V$. For an open residual set $V_k$ of positive finite measure, [inner regularity of Lebesgue measure](../../../../../inner-regularity-of-lebesgue-measure.md) supplies a compact $K_k\subseteq V_k$ with $\lambda_d(K_k)\geq\lambda_d(V_k)/2$. Cover $K_k$ by finitely many open balls whose closures lie in $V_k$, and use the [Wiener covering lemma](../../../../../wiener-covering-lemma.md) to select disjoint balls. Their total measure is at least $\lambda_d(V_k)/(2\cdot3^d)$. Remove their closures to obtain the open residual set $V_{k+1}$. Ball boundaries are [null sets](../../../../../null-set.md), so

$$
\lambda_d(V_{k+1})\leq\left(1-\frac1{2\cdot3^d}\right)\lambda_d(V_k).
$$

All retained balls, including those from different stages, are pairwise disjoint and contained in $V$. They form a countable family. The uncovered set is contained in $\bigcap_kV_k$ together with their countably many boundaries, and both have measure zero. Enumerating the retained balls gives

$$
\boxed{\lambda_d\left(V\setminus\bigcup_nU_n\right)=0.}
$$

Next consider the [uncentered maximal function of a finite measure](../../../../../uncentered-maximal-function-of-a-finite-measure.md). For every real $\alpha$, its strict superlevel set is

$$
\{x:m_u(x)>\alpha\}
=\bigcup_{\mu(U_r(y))>\alpha\lambda_d(U_r(y))}U_r(y).
$$

Indeed, membership in the ball is exactly the strict condition $\|x-y\|<r$ in the supremum. This union is open, proving that $m_u$ is [lower semicontinuous](../../../../../lower-semicontinuity.md) as an extended nonnegative function; it may take the value infinity.

For $\alpha>0$, take a compact subset $K$ of this superlevel set and choose a finite cover by balls satisfying the displayed density inequality. The [Wiener covering lemma](../../../../../wiener-covering-lemma.md) selects disjoint balls $B_j$ whose triples cover $K$. Since $\mu$ is a [probability measure](../../../../../probability-measure.md),

$$
\lambda_d(K)\leq3^d\sum_j\lambda_d(B_j)
<\frac{3^d}{\alpha}\sum_j\mu(B_j)\leq\frac{3^d}{\alpha}.
$$

Take the supremum over compact $K$ using [inner regularity of Lebesgue measure](../../../../../inner-regularity-of-lebesgue-measure.md). This works even if the open superlevel set was initially unbounded, and proves the [uncentered maximal weak-type inequality](../../../../../uncentered-maximal-weak-type-inequality.md)

$$
\boxed{\lambda_d\{m_u>\alpha\}\leq\frac{3^d}{\alpha}.}
$$

For a finite positive measure of mass $M$, scaling gives $3^dM/\alpha$ instead.

One important use is the [Lebesgue differentiation theorem](../../../../../lebesgue-differentiation-theorem.md). For $f\in L^1(\mathbb R^d)$, approximate it in $L^1$ by a compactly supported continuous $g$, and set $h=|f-g|$. The limiting mean oscillation of $f$ at $x$ is at most $m_{h\lambda_d}(x)+h(x)$, since that of $g$ vanishes by continuity. The preceding weak-type estimate and the elementary integral bound on $\{h>t\}$ give

$$
\lambda_d\{\text{limiting mean oscillation}>2t\}
\leq\frac{3^d+1}{t}\|f-g\|_1.
$$

Let the approximation error tend to zero and then take countably many $t\downarrow0$. The local averages of $f$ converge to $f(x)$ almost everywhere. Localizing extends this to locally integrable functions. Thus the maximal estimate turns norm approximation by [continuous functions](../../../../../continuous-function.md) into almost-everywhere information about local averages.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
