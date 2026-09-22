<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [dual space](../../../../dual-space-split.md) $X'$ consists of bounded linear maps $g:X\to\mathbb C$, with [operator norm](../../../../operator-norm.md) $\|g\|=\sup_{\|x\|\leq1}|g(x)|$. It is Banach even if $X$ is not: an operator-[norm](../../../../norm.md) [Cauchy sequence](../../../../cauchy-sequence.md) has pointwise limits, these define a [bounded linear functional](../../../../continuous-linear-functional.md), and the uniform Cauchy estimate on the unit ball gives operator-[norm](../../../../norm.md) convergence.

Restriction $R(g)=g|_Z$ is linear and contractive. If $Z$ is [dense](../../../../dense-set.md), for every $x\in X$ choose $z_n\in Z$ with $z_n\to x$. The bound $|g(z_n)|\leq\|Rg\|\|z_n\|$ passes to the limit, proving $|g(x)|\leq\|Rg\|\|x\|$. Hence $\|g\|=\|Rg\|$ and restriction is [injective](../../../../injective-function.md). Conversely, for $h\in Z'$ define $g(x)=\lim h(z_n)$. The estimate $|h(z_n)-h(z_k)|\leq\|h\|\|z_n-z_k\|$ gives existence and independence of the approximating sequence. It also gives linearity and $\|g\|\leq\|h\|$. Thus **restriction is an onto linear [isometry](../../../../isometry.md) of dual spaces**.

For the sequence subspace in this part, the [norm](../../../../norm.md) is the unweighted $\ell^1$ [norm](../../../../norm.md); only its membership condition uses the weight $j$. It contains all finitely supported sequences, hence is [dense](../../../../dense-set.md) in $\ell^1$. Applying restriction to $X=\ell^1$ and using its known dual yields

$$
\boxed{Z'\cong\ell^\infty\text{ isometrically},\qquad h_b(\alpha)=\sum_{j=1}^\infty b_j\alpha_j,\quad\|h_b\|=\|b\|_\infty.}
$$

## ↑ Ancestors (12)

1. [2](../2.md)
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
