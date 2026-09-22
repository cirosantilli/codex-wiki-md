<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [norm](../../../../norm.md)-preserving form of the [Hahn-Banach theorem](../../../../hahn-banach-theorem.md) states: if $M$ is a [linear subspace](../../../../vector-subspace.md) of a real or complex [normed vector space](../../../../normed-vector-space-split.md) $X$ and $f:M\to\mathbb K$ is a bounded [linear functional](../../../../linear-functional.md), there exists $F\in X^*$ with $F|_M=f$ and $\|F\|=\|f\|$.

For a real [separable](../../../../separable-topological-space.md) $X$, put $C=\|f\|$. The case $C=0$ is immediate. To extend over one vector $x_0\notin M$, choose a real number $c$ between

$$
\sup_{m\in M}\bigl(f(m)-C\|m-x_0\|\bigr)
\quad\text{and}\quad
\inf_{n\in M}\bigl(C\|n+x_0\|-f(n)\bigr).
$$

The lower endpoint is no greater than the upper: for any $m,n\in M$,

$$
f(m)+f(n)=f(m+n)\leq C\|m+n\|\leq C\|m-x_0\|+C\|n+x_0\|.
$$

The endpoints are finite because testing zero bounds them between finite numbers. Define $F(m+tx_0)=f(m)+tc$. The upper inequality ensures $F(z)\leq C\|z\|$ for vectors with positive $x_0$ coefficient, and the lower inequality gives it for negative coefficient; it already holds on $M$. Applying the same bound to $-z$ gives $|F(z)|\leq C\|z\|$. Thus the extension preserves the [norm](../../../../norm.md).

Now add a countable dense sequence of vectors one at a time. The consistent extensions define a bounded functional of [norm](../../../../norm.md) $C$ on the union of the increasing domains. That union is dense in $X$, so extension by [continuity](../../../../continuous-function.md) gives the desired functional on all of $X$. This proves the real [separable](../../../../separable-topological-space.md) case without a maximality argument.

For the density application, suppose the [closed linear span](../../../../closed-linear-span.md) $M$ were proper. The [Hahn-Banach theorem](../../../../hahn-banach-theorem.md) supplies a nonzero continuous [linear functional](../../../../linear-functional.md) annihilating $M$. By [duality of sequence spaces](../../../../duality-of-sequence-spaces.md), it has the form $f(z)=\sum_{j\geq1}a_jz_j$ with $a\in\ell_1$, not identically zero. Let $m$ be the first index with $a_m\ne0$. Writing $t_n=(n+1)^{-1}$, annihilation of $x_n$ gives

$$
0=t_n^{-m}f(x_n)=a_m+\sum_{j>m}a_jt_n^{j-m}.
$$

The tail has absolute value at most $t_n\sum_{j>m}|a_j|\to0$. Letting $n\to\infty$ contradicts $a_m\ne0$. Therefore

$$
\boxed{\overline{\operatorname{span}}\{x_n:n\geq1\}=c_0.}
$$

This is [geometric sequences with accumulating ratios span c0](../../../../geometric-sequences-with-accumulating-ratios-span-c0.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
