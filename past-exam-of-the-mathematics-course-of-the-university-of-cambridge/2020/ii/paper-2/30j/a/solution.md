<h1 id="30j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A sample $x_{1:n}=(x_1,\ldots,x_n)$ is shattered by $\mathcal F$ when every binary labeling is realized:

$$
\{(f(x_1),\ldots,f(x_n)):f\in\mathcal F\}=\{0,1\}^n.
$$

The [shattering coefficient](../../../../../../shattering-coefficient.md) and [VC dimension](../../../../../../vc-dimension.md) are

$$
s(\mathcal F,n)
=\sup_{x_{1:n}\in\mathcal X^n}
\left|\{(f(x_1),\ldots,f(x_n)):f\in\mathcal F\}\right|,
$$



$$
\operatorname{VC}(\mathcal F)
=\sup\{n:s(\mathcal F,n)=2^n\}.
$$

For the lower orthants in $\mathbb R^d$, the $d$ points $e_1,\ldots,e_d$ are shattered: to realize a subset $I$, choose $a_j=1$ for $j\in I$ and $a_j=1/2$ otherwise. Conversely, among any $d+1$ points choose, for each coordinate, one point attaining the maximum in that coordinate. At most $d$ points have been chosen, so there is an unchosen point $x$. Any lower orthant containing every chosen coordinate maximizer must contain every sample point, including $x$. It cannot realize the labeling that includes all chosen points and excludes $x$. This proves

$$
\boxed{\operatorname{VC}(\mathcal F)=d}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30J](../../30j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
