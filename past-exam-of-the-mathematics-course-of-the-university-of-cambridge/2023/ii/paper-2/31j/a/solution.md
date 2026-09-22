<h1 id="31j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For fixed sample points $x_{1:n}=(x_1,\ldots,x_n)$, write

$$
\mathcal H(x_{1:n})
=\{(h(x_1),\ldots,h(x_n)):h\in\mathcal H\}.
$$

The [shattering coefficient](../../../../../../shattering-coefficient.md) is

$$
\boxed{s(\mathcal H,n)=\sup_{x_{1:n}\in\mathcal X^n}|\mathcal H(x_{1:n})|.}
$$

Thus it is the largest number of distinct binary labelings that the [hypothesis class](../../../../../../concept-class.md) can realize on $n$ points.

A set of $n$ points is shattered when all $2^n$ labelings are realized. The [VC dimension](../../../../../../vc-dimension.md) is therefore

$$
\boxed{\operatorname{VC}(\mathcal H)
=\sup\{n:s(\mathcal H,n)=2^n\},}
$$

with value infinity if arbitrarily large finite sets are shattered.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31J](../../31j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
