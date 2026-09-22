<h1 id="21f/solution">Solution</h1>

↑ **Parent:** [21F](../21f.md)

The [continuous dual space](../../../../../continuous-dual-space-split.md) $X^*$ consists of bounded complex-linear functionals $\phi:X\to\mathbb C$, with $\|\phi\|=\sup_{\|x\|\leq1}|\phi(x)|$. For $1\leq s<\infty$, $\ell^s$ consists of sequences with $\sum_j|x_j|^s<\infty$, [norm](../../../../../norm.md) $(\sum_j|x_j|^s)^{1/s}$; $\ell^\infty$ consists of bounded sequences with supremum [norm](../../../../../norm.md).

For $a\in\ell^p$, define $\phi_a(x)=\sum_j a_jx_j$ on $\ell^q$. [Hölder's inequality](../../../../../holder-s-inequality.md) gives absolute convergence and $\|\phi_a\|\leq\|a\|_p$. For a finite truncation, choose $x_j=\overline{a_j}|a_j|^{p-2}/(\sum_{j\leq N}|a_j|^p)^{1/q}$ for $j\leq N$, zero elsewhere, interpreting the numerator as zero when $a_j=0$. Its $q$-norm is one and its pairing equals $(\sum_{j\leq N}|a_j|^p)^{1/p}$. Letting $N$ grow proves equality of the [norms](../../../../../norm.md).

Conversely, for a bounded $\phi$ let $a_j=\phi(e_j)$. The same finite test vector gives $\sum_{j\leq N}|a_j|^p\leq\|\phi\|^p$, so $a\in\ell^p$. Finite truncations converge in $\ell^q$, and continuity gives $\phi(x)=\sum_j a_jx_j$. Thus $\boxed{(\ell^q)^*\cong\ell^p\text{ isometrically}.}$

For $\ell^1$, boundedness gives $|a_j|\leq\|\phi\|$, while any bounded sequence defines an absolutely convergent pairing bounded by $\|a\|_\infty\|x\|_1$. Density of finite sequences again proves surjectivity, and single-coordinate tests give [norm](../../../../../norm.md) equality. Hence $\boxed{(\ell^1)^*\cong\ell^\infty\text{ isometrically}.}$ The reversed argument fails for $\ell^\infty$: finite sequences are not dense in its supremum [norm](../../../../../norm.md); their closure is $c_0$. For example the limit functional on convergent sequences extends by the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) to $\ell^\infty$, vanishes on every $e_j$, yet takes value one on the constant-one sequence. It cannot be represented by pairing with an $\ell^1$ coefficient sequence.

## ↑ Ancestors (10)

1. [21F](../21f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
