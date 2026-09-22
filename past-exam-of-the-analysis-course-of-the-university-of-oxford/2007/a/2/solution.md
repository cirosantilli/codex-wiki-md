<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [continuous dual space](../../../../continuous-dual-space-split.md) $X'$ consists of all bounded complex-linear [functionals](../../../../functional.md) $f:X\to\mathbb C$, with pointwise vector operations and [norm](../../../../norm.md) $\|f\|=\sup_{\|x\|\leq1}|f(x)|$. This is finite by boundedness. The scalar [norm](../../../../norm.md) identity and [triangle inequality](../../../../triangle-inequality.md) follow under the supremum; if the [norm](../../../../norm.md) is zero, scaling every nonzero vector into the unit ball shows that $f$ vanishes. Hence $X'$ is a normed [complex vector space](../../../../complex-vector-space.md).

For the [dual of the convergent sequence space](../../../../dual-of-the-convergent-sequence-space.md), take $\beta\in\ell^1$. The displayed formula is a [bounded linear functional](../../../../continuous-linear-functional.md), since the [series](../../../../series-mathematics.md) is absolutely convergent and

$$
|\phi(\beta)(\alpha)|\leq\left(|\beta_1|+\sum_{j\geq1}|\beta_{j+1}|\right)\|\alpha\|_\infty.
$$

It is linear in $\beta$, so $\|\phi(\beta)\|\leq\|\beta\|_1$. For equality fix $N$, choose $\alpha_j$ for $j\leq N$ of modulus at most one so that $\alpha_j\beta_{j+1}=|\beta_{j+1}|$, and make all later terms equal a constant $c$ of modulus at most one with $c\beta_1=|\beta_1|$. The choices for a zero coefficient can be arbitrary. This sequence lies in the unit ball of $c$ and converges to $c$. The [reverse triangle inequality](../../../../reverse-triangle-inequality.md) gives

$$
|\phi(\beta)(\alpha)|\geq|\beta_1|+\sum_{j=1}^N|\beta_{j+1}|-\sum_{j>N}|\beta_{j+1}|.
$$

Letting $N\to\infty$ proves **$\|\phi(\beta)\|=\|\beta\|_1$**, including injectivity.

For surjectivity let $F\in c'$. By the permitted description of $c_0'$, there is $\gamma\in\ell^1$ with $F(z)=\sum_j\gamma_jz_j$ on $c_0$. Every $\alpha\in c$ decomposes as $\alpha-\alpha_\infty\mathbf1\in c_0$ plus $\alpha_\infty\mathbf1$. Consequently

$$
F(\alpha)=\sum_j\gamma_j\alpha_j+\alpha_\infty\left(F(\mathbf1)-\sum_j\gamma_j\right).
$$

Take $\beta_{j+1}=\gamma_j$ and $\beta_1=F(\mathbf1)-\sum_j\gamma_j$. This is an $\ell^1$ sequence and $F=\phi(\beta)$, proving **the stated isometric linear isomorphism onto $c'$**. No complex conjugation is inserted, since these are complex-linear dual [functionals](../../../../functional.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
