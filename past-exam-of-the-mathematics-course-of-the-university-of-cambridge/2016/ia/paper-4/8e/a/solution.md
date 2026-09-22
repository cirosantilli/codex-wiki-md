<h1 id="8e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First establish the [binomial theorem](../../../../../../binomial-theorem.md) needed throughout this question. For integers $0\leq m\leq n$, define the [binomial coefficient](../../../../../../binomial-coefficient.md) $\binom nm$ to be the number of $m$-element [subsets](../../../../../../subset.md) of an $n$-element set. Counting ordered selections and then forgetting their order gives

$$
\binom nm=\frac{n!}{m!(n-m)!},
$$

with the [factorial](../../../../../../factorial.md) convention $0!=1$. In the product of $n$ factors $(1+z)$, choose $z$ from exactly $m$ factors and $1$ from the others. Each choice contributes $z^m$, and there are $\binom nm$ choices. The distributive law therefore proves

$$
(1+z)^n=\sum_{m=0}^n\binom nm z^m
$$

for every [complex number](../../../../../../complex-number.md) $z$, including $n=0$ by the empty-product convention.

To evaluate the even-indexed sum, use the [even part of a polynomial](../../../../../../even-part-of-a-polynomial.md): averaging the [binomial theorem](../../../../../../binomial-theorem.md) at $z$ and $-z$ cancels the odd powers. For $z=i\sqrt3$,

$$
\sum_{k=0}^{3n}(-3)^k\binom{6n}{2k}
=\frac{(1+i\sqrt3)^{6n}+(1-i\sqrt3)^{6n}}2.
$$

The two [complex numbers](../../../../../../complex-number.md) satisfy $1\pm i\sqrt3=2e^{\pm i\pi/3}$. Their $6n$th powers are both $2^{6n}$, since $e^{\pm2\pi in}=1$. Thus **the sum is**

$$
\boxed{2^{6n}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
