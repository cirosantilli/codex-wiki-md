<h1 id="12f/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Write $N=\sum_iI_i$ as in part (ii). For $i\ne j$, the two vertices are both isolated exactly when their combined $2n-3$ incident edges are absent, so

$$
\mathbb E(I_iI_j)=(1-p)^{2n-3}.
$$

Therefore

$$
\boxed{
\mathbb E(N^2)
=n(1-p)^{n-1}
+n(n-1)(1-p)^{2n-3}.
}
$$

Let $A=\mathbb EN=n(1-p)^{n-1}$. The displayed formula gives

$$
\frac{\operatorname{var}(N)}{A^2}
=\frac1A+\frac{n-1}{n(1-p)}-1
=\frac1A+\frac{p-1/n}{1-p}.
$$

Now take $p=c\log n/n$ with $c<1$, and choose $\alpha>1$ such that $\alpha c<1$. For all sufficiently large $n$, the supplied inequality gives $1-p\geq e^{-\alpha p}$, whence

$$
A\geq ne^{-\alpha p(n-1)}
=n^{\,1-\alpha c(n-1)/n}
\longrightarrow\infty.
$$

Also $p\to0$, so both terms in the variance ratio tend to zero. Part (iv) now applies and proves the lower side of the isolated-vertex threshold:

$$
\boxed{\mathbb P(N=0)\longrightarrow0}.
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
