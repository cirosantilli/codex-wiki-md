<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

If $(a^{(n)})$ is Cauchy in the [maximum norm](../../../../supremum-norm.md) on $\mathbb C^m$, every coordinate is Cauchy in $\mathbb C$ and has a limit $a_j$. Given $\varepsilon>0$, for sufficiently large $n,k$ every coordinate difference is at most $\varepsilon$. Letting $k\to\infty$ gives $\max_j|a_j^{(n)}-a_j|\leq\varepsilon$. Thus **$\mathbb C^m$ with its [maximum norm](../../../../supremum-norm.md) is [complete](../../../../completeness.md)**.

Let $F(a)=\sum a_jz_j$. The [triangle inequality](../../../../triangle-inequality.md) gives

$$
\|F(a)\|\leq\left(\sum_{j=1}^m\|z_j\|\right)\|a\|_\infty.
$$

Take $\delta=\sum\|z_j\|$. This estimate also makes $a\mapsto\|F(a)\|$ [continuous](../../../../continuous-function.md) on the maximum-[norm](../../../../norm.md) unit sphere, which is [compact](../../../../compact-space.md) by coordinatewise Bolzano-Weierstrass. [Linear independence](../../../../linear-independence.md) makes this function strictly positive there, so its minimum $\gamma$ is positive. [Homogeneity](../../../../homogeneity.md) then gives

$$
\boxed{\gamma\|a\|_\infty\leq\|F(a)\|\leq\delta\|a\|_\infty.}
$$

A [Cauchy sequence](../../../../cauchy-sequence.md) in $X$ consequently has Cauchy coordinate vectors in $\mathbb C^m$. Their coordinate limit maps by the upper estimate to a limit in $X$. Therefore **every finite-dimensional normed complex space is a [Banach space](../../../../banach-space-split.md)**.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
