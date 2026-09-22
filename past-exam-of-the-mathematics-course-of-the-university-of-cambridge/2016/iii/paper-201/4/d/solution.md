<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mu$ be the given [Brownian motion](../../../../../../brownian-motion-split.md) law on $C[0,1]$. Choose $\alpha<\beta<1/2$ and an integer $p$ with $p(1/2-\beta)>1$. For the largest adjacent level-$n$ increment $A_n$, [Brownian scaling](../../../../../../brownian-scaling.md) and the [Markov inequality](../../../../../../markov-inequality.md) give

$$
\mu(A_n>2^{-n\beta})
\leq\sum_{k=0}^{2^n-1}\frac{\mathbb E|X_{(k+1)2^{-n}}-X_{k2^{-n}}|^p}{2^{-np\beta}}
=c_p\,2^{-n(p(1/2-\beta)-1)},
$$

where $c_p=\mathbb E|\mathcal N(0,1)|^p<\infty$. These probabilities are summable, so the [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) gives a finite random $K$ such that $A_n\leq K2^{-n\beta}$ for every $n$, after absorbing the finitely many exceptional levels.

For $s<t$, choose $m$ with $2^{-m}\leq t-s<2^{1-m}$. Their left dyadic approximations at level $m$ differ by at most two grid steps; each finer approximation adds at most one adjacent increment. Continuity and [dyadic increment chaining](../../../../../../dyadic-increment-chaining.md) therefore give

$$
|X_t-X_s|\leq2\sum_{j\geq m}A_j
\leq\frac{2K}{1-2^{-\beta}}\,2^{-m\beta}
\leq\frac{2K}{1-2^{-\beta}}(t-s)^\beta.
$$

Thus paths are $\beta$-Hölder and hence $\alpha$-Hölder on $[0,1]$. This direct proof supplies the relevant [Brownian Hölder regularity](../../../../../../brownian-holder-regularity.md), also obtainable from the [Kolmogorov continuity theorem](../../../../../../kolmogorov-continuity-theorem.md).

The full-measure subset $E_\alpha=C^\alpha[0,1]$ is measurable in $C[0,1]$, because continuity identifies its seminorm with a countable supremum:

$$
\|w\|_\alpha
=\sup_{s<t,\ s,t\in\mathbb Q\cap[0,1]}
\frac{|w(t)-w(s)|}{(t-s)^\alpha}.
$$

Its finiteness event is a countable union of countable intersections of coordinate-measurable events. The sigma-algebra specified on $E_\alpha$ is precisely the trace of the [coordinate sigma-algebra](../../../../../../cylinder-sigma-algebra.md) on $C[0,1]$. Define $\nu(A)=\mu(A)$ for trace-measurable $A\subseteq E_\alpha$; equivalently restrict the Brownian law to its full-measure subset. Since $\mu(E_\alpha)=1$, no renormalization is needed, and all finite-dimensional coordinate laws are unchanged. **This is the required [probability measure](../../../../../../probability-measure.md)**:

$$
\boxed{\nu(C^\alpha[0,1])=1,\qquad (X_t)_{0\leq t\leq1}\text{ is Brownian under }\nu.}
$$

The construction uses the requested coordinate sigma-algebra and makes no assumption about a separable Hölder-norm topology.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
