<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Equip the [continuous dual space](../../../../../continuous-dual-space-split.md) $X'$ with the [operator norm](../../../../../operator-norm.md)

$$
\|f\|=\sup_{\|x\|\leq1}|f(x)|.
$$

[Continuity](../../../../../continuous-function.md) of a [linear functional](../../../../../linear-functional.md) makes this finite; homogeneity, definiteness and the [triangle inequality](../../../../../triangle-inequality.md) follow directly from the supremum formula.

For [completeness of the dual space](../../../../../completeness-of-the-dual-space.md), let $(f_n)$ be Cauchy in this [norm](../../../../../norm.md). For each $x\in X$, $|f_n(x)-f_m(x)|\leq\|f_n-f_m\|\|x\|$, so $(f_n(x))$ is Cauchy in $\mathbb R$. Define $f(x)=\lim_nf_n(x)$. Passing to the limit in the linearity identities makes $f$ linear. Since a [Cauchy sequence](../../../../../cauchy-sequence.md) is bounded, $\sup_n\|f_n\|\leq C$ and $|f(x)|\leq C\|x\|$, so $f\in X'$.

Given $\varepsilon>0$, choose $N$ with $\|f_n-f_m\|\leq\varepsilon$ for $n,m\geq N$. Let $m\to\infty$ [pointwise](../../../../../pointwise-convergence.md); then $|f_n(x)-f(x)|\leq\varepsilon\|x\|$ and therefore $\|f_n-f\|\leq\varepsilon$. Thus **$X'$ is a [Banach space](../../../../../banach-space-split.md)**. This proof in fact works even if $X$ itself is not complete.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
