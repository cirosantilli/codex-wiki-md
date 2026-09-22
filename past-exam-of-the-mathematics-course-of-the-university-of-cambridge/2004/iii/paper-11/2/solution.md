<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [asymmetric Lovász local lemma](../../../../../asymmetric-lovasz-local-lemma.md) says the following. For finitely many bad [events](../../../../../event.md) with a [dependency graph of events](../../../../../dependency-graph-of-events.md), if $0\leq x_i<1$ satisfy

$$
\Pr(A_i)\leq x_i\prod_{j\in\Gamma(i)}(1-x_j),
$$

then

$$
\boxed{\Pr\left(\bigcap_i A_i^c\right)\geq\prod_i(1-x_i)>0.}
$$

Here independence from nonneighbors is independence from their whole generated system, not just pairwise independence.

Prove by induction on $|S|$ that $\Pr(A_i\mid\bigcap_{j\in S}A_j^c)\leq x_i$ whenever $i\notin S$, with all conditioning [probabilities](../../../../../probability.md) positive. At $S=\varnothing$, the hypothesis gives $\Pr(A_i)\leq x_i$. Split $S$ into its neighbor part $S_1$ and nonneighbor part $S_2$. Then

$$
\begin{aligned}
\Pr(A_i\mid\bigcap_{j\in S}A_j^c)
&\leq\frac{\Pr(A_i\mid\bigcap_{j\in S_2}A_j^c)}
{\Pr(\bigcap_{j\in S_1}A_j^c\mid\bigcap_{j\in S_2}A_j^c)}\\
&\leq\frac{\Pr(A_i)}{\prod_{j\in S_1}(1-x_j)}\leq x_i.
\end{aligned}
$$

The numerator uses joint nonneighbor independence. The denominator is exposed one [event](../../../../../event.md) at a time; every conditional bad-event [probability](../../../../../probability.md) involves fewer than $|S|$ conditioning [events](../../../../../event.md), so induction supplies the product lower bound. The same product argument gives positivity of the conditioning [events](../../../../../event.md) before using the fraction. Finally expose all complements in any order and multiply their conditional [probabilities](../../../../../probability.md) to obtain the claimed lower bound.

For maximum dependency degree $d\geq1$ and [event](../../../../../event.md) [probabilities](../../../../../probability.md) at most $p$, choose $x_i=1/(d+1)$. Since $(1+1/d)^d\leq e$, the symmetric [Lovász local lemma](../../../../../lovasz-local-lemma.md) follows from

$$
\boxed{ep(d+1)\leq1.}
$$

For $d=0$, the [events](../../../../../event.md) are jointly independent and avoidance has positive [probability](../../../../../probability.md) whenever $p<1$, so the displayed sufficient criterion also holds.

To obtain the [local lemma Ramsey lower bound](../../../../../local-lemma-ramsey-lower-bound.md), colour the edges of $K_N$ independently with two equally likely colours. For every $k$-set $S$, the [event](../../../../../event.md) that it is monochromatic has [probability](../../../../../probability.md) $p=2^{1-\binom k2}$. [Events](../../../../../event.md) with intersections of size at most one depend on disjoint edge trials. Counting potentially shared pairs gives

$$
d\leq\binom k2\binom{N-2}{k-2}.
$$

The [Lovász local lemma](../../../../../lovasz-local-lemma.md) excludes all monochromatic $K_k$ if $ep(d+1)\leq1$. For $N\leq ck2^{k/2}$, [Stirling's approximation](../../../../../stirling-formula.md) and $\binom{N-2}{k-2}\leq N^{k-2}/(k-2)!$ give, uniformly for $c$ bounded above and away from zero,

$$
ep(d+1)=O\left(k^{3/2}\left(\frac{ec}{\sqrt2}\right)^k\right)+o(1).
$$

For a concrete approach to the limiting constant, choose $c_k=(\sqrt2/e)(1-3\log k/k)$ and take the integer part of $c_kk2^{k/2}$. Then $(ec_k/\sqrt2)^k\leq k^{-3}$ for all sufficiently large $k$, so the criterion holds. Such a colouring shows $R(k)>N$, and therefore

$$
\boxed{R(k)\geq(\sqrt2/e+o(1))k2^{k/2}.}
$$

The undefined $o(i)$ printed in the PDF is read as the intended $o(1)$, with $k\to\infty$.

For the cycle, independently choose one of the twelve vertices in each part. Ignore cycle edges whose endpoints lie in the same part, since both endpoints cannot be selected. Every other edge defines a bad [event](../../../../../event.md) of [probability](../../../../../probability.md) $1/144$. It uses just the choices in its two endpoint parts. A part's twelve vertices meet at most twenty-four cycle edges, so a bad [event](../../../../../event.md) has at most $48-1=47$ neighbors in a [dependency graph of events](../../../../../dependency-graph-of-events.md). Since $e(47+1)/144=e/3<1$, the [Lovász local lemma](../../../../../lovasz-local-lemma.md) gives a selection with no selected adjacent pair. Thus **an independent transversal of size $n$ exists**, for every stated partition.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
