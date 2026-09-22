<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the intended space of [Hilbert-Schmidt operators](../../../../../hilbert-schmidt-operator.md), with the given [Hilbert-Schmidt inner product](../../../../../hilbert-schmidt-inner-product.md) linear in its first argument. It remains to prove completeness in its [Hilbert-Schmidt norm](../../../../../hilbert-schmidt-norm.md). Let $(T_n)$ be a [Cauchy sequence](../../../../../cauchy-sequence.md) in that [norm](../../../../../norm.md). The bound $\|T_n-T_m\|\leq\|T_n-T_m\|_2$ makes it a [Cauchy sequence](../../../../../cauchy-sequence.md) in [operator norm](../../../../../operator-norm.md). The space $\mathcal B(X)$ is a [Banach space](../../../../../banach-space-split.md), so $T_n\to T$ in [operator norm](../../../../../operator-norm.md) for some [bounded linear operator](../../../../../continuous-linear-operator.md) $T$.

For completeness, that last standard fact follows by taking $Tx=\lim_nT_nx$ for each $x$: the [Cauchy sequence](../../../../../cauchy-sequence.md) $(T_n)$ is uniformly bounded in [operator norm](../../../../../operator-norm.md), so its limit is linear and bounded, and the uniform Cauchy estimate on the [unit ball](../../../../../unit-ball.md) gives [operator norm](../../../../../operator-norm.md) convergence.

Given $\varepsilon>0$, choose $N$ so that $\|T_n-T_m\|_2<\varepsilon$ for $n,m\geq N$. Fix $n\geq N$ and any positive integer $K$. Since $T_me_k\to Te_k$ for each $k$, passage to the limit in a finite sum gives

$$
\sum_{k=1}^K\|(T_n-T)e_k\|^2
=\lim_{m\to\infty}\sum_{k=1}^K\|(T_n-T_m)e_k\|^2
\leq\varepsilon^2.
$$

Taking the supremum over $K$ gives $\sum_k\|(T_n-T)e_k\|^2\leq\varepsilon^2$. Also,

$$
\sum_k\|Te_k\|^2
\leq2\sum_k\|T_Ne_k\|^2+2\sum_k\|(T-T_N)e_k\|^2<\infty.
$$

Thus $T\in S_2(X)$, and $\|T_n-T\|_2\leq\varepsilon$ for $n\geq N$. This proves [Hilbert-Schmidt operators form a Hilbert space](../../../../../hilbert-schmidt-operators-form-a-hilbert-space.md):

$$
\boxed{S_2(X)\text{ is complete in }\|\cdot\|_2,\text{ hence is a Hilbert space}.}
$$

Under the literal unrestricted “linear mappings” definition, the nonzero $R$ from part (i) satisfies $\langle R,R\rangle_{S_2(X)}=0$. The form would fail positive definiteness and would not be an [inner product](../../../../../inner-product-split.md); the boundedness correction is needed here too.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
