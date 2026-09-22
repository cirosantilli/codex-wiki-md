<h1 id="22f/solution">Solution</h1>

↑ **Parent:** [22F](../22f.md)

Concavity of $\log$ gives $\log(a/p+b/q)\geq p^{-1}\log a+q^{-1}\log b$ because $1/p+1/q=1$. Exponentiating proves [Young inequality](../../../../../young-s-inequality-for-products.md)

$$
\boxed{a^{1/p}b^{1/q}\leq a/p+b/q,}
$$

with equality precisely when $a=b$. Equivalently it follows from convexity of the exponential.

Define $\ell^p=\{x=(x_j):\sum_j|x_j|^p<\infty\}$ with $\|x\|_p=(\sum_j|x_j|^p)^{1/p}$. Positivity, definiteness and homogeneity are immediate. Summing [Young inequality](../../../../../young-s-inequality-for-products.md) for normalized sequences gives [Hölder's inequality](../../../../../holder-s-inequality.md) $\sum|x_jy_j|\leq\|x\|_p\|y\|_q$. For a finite truncation $z=x+y$, it yields

$$
\sum|z_j|^p\leq\sum(|x_j|+|y_j|)|z_j|^{p-1}
\leq(\|x\|_p+\|y\|_p)\left(\sum|z_j|^p\right)^{1/q}.
$$

Dividing and passing to larger truncations proves [Minkowski inequality](../../../../../minkowski-inequality.md) and shows $x+y\in\ell^p$, so this is a [normed vector space](../../../../../normed-vector-space.md).

Let $x^{(m)}$ be a norm-Cauchy sequence. Each coordinate is Cauchy because $|x_j^{(m)}-x_j^{(l)}|\leq\|x^{(m)}-x^{(l)}\|_p$, and let its limit be $x_j$. The sequence [norms](../../../../../norm.md) are bounded by some $C$. For every finite $N$, passage to coordinate limits gives $\sum_{j\leq N}|x_j|^p\leq C^p$, so $x\in\ell^p$. Given $\varepsilon>0$, choose $M$ with $\|x^{(m)}-x^{(l)}\|_p<\varepsilon$ for $m,l\geq M$. Letting $l\to\infty$ in finite truncations and then $N\to\infty$ gives $\|x^{(m)}-x\|_p\leq\varepsilon$ for $m\geq M$. **Thus $\ell^p$ is complete, hence a [Banach space](../../../../../banach-space-split.md).**

## ↑ Ancestors (10)

1. [22F](../22f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
