<h1 id="22i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Baire category theorem](../../../../../../baire-category-theorem.md) says that a complete metric space cannot be a countable union of [nowhere dense sets](../../../../../../nowhere-dense-set.md), equivalently that every countable intersection of open dense sets is dense. To prove it, let $G_1,G_2,\ldots$ be open dense subsets and let $V$ be nonempty and open. Choose nested closed balls

$$
\overline B(x_n,r_n)\subset B(x_{n-1},r_{n-1})\cap G_n,
\qquad 0<r_n<2^{-n},
$$

starting inside $V\cap G_1$. The centres are a [Cauchy sequence](../../../../../../cauchy-sequence.md); completeness gives a limit lying in every ball, hence in $V\cap\bigcap_nG_n$. Thus the intersection is dense.

Choose a countable sequence $q_j\uparrow p$ with $1\le q_j<p$. Since $\ell^q\subset\ell^r$ for $q<r$, every $\ell^q$ with $q<p$ lies in some $\ell^{q_j}$. For integers $m\ge1$, set

$$
E_{j,m}=\{x\in\ell^p:\|x\|_{q_j}\le m\}.
$$

Pointwise convergence and [Fatou lemma for series](../../../../../../fatou-lemma-for-series.md) show that $E_{j,m}$ is closed in $\ell^p$. It has empty interior: inside any $\ell^p$ ball, add a sufficiently long finite block whose $\ell^p$ norm is tiny but whose $\ell^{q_j}$ norm is larger than $m$. Therefore every $E_{j,m}$ is nowhere dense. Since $\ell^p$ is a [Banach space](../../../../../../banach-space-split.md), Baire gives

$$
\ell^p\ne\bigcup_{j,m}E_{j,m}
=\bigcup_{1\le q<p}\ell^q.
$$

An explicit element of the difference is

$$
\boxed{x_n=\frac1{n^{1/p}\{\log(n+1)\}^{2/p}}}.
$$

Its $p$th powers form a convergent logarithmic series, whereas for every $q<p$ the powers contain $n^{-q/p}$ with exponent below one and their series diverges. Hence $x\in\ell^p$ but $x\notin\ell^q$ for every $q<p$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22I](../../22i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
