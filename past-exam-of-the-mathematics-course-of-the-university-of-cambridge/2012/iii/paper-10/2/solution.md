<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Clear a common denominator first, so that all coefficients are nonzero integers. This changes neither the solutions nor [partition regularity](../../../../../partition-regular-matrix.md). We prove the one-equation criterion directly; no form of [Rado's theorem](../../../../../rado-s-theorem.md) is used as an assumption.

For necessity, choose a [prime number](../../../../../prime-number.md) $p>\sum_i|a_i|$. Colour a positive integer by its first nonzero base-$p$ digit: writing $x=p^{v_p(x)}u$ with $p\nmid u$, use the colour $u\pmod p\in\{1,\ldots,p-1\}$. Suppose the equation has a [monochromatic](../../../../../monochromatic-set.md) solution. Let $v$ be the smallest [P-adic valuation](../../../../../p-adic-valuation.md) of its entries and put $I=\{i:v_p(x_i)=v\}$, a nonempty set. Divide the equation by $p^v$ and reduce modulo $p$. All entries indexed by $I$ contribute the same nonzero digit $u$, and all other terms vanish. Hence

$$
u\sum_{i\in I}a_i\equiv0\pmod p.
$$

It follows that $p$ divides $\sum_{i\in I}a_i$. The absolute value of this sum is less than $p$, so **$\boxed{\sum_{i\in I}a_i=0}$**.

For sufficiency, take a nonempty zero-sum index set $I$ and put $S=\sum_{i\notin I}a_i$. If $S=0$, the full coefficient sum is zero and the constant vector $(1,\ldots,1)$ is already a [monochromatic](../../../../../monochromatic-set.md) solution in every colouring. Otherwise choose $j\in I$, put $t=|a_j|$, and set $b_j=-\operatorname{sgn}(a_j)S$, $b_i=0$ for $i\in I\setminus\{j\}$. Then

$$
\sum_{i\in I}a_ib_i=-tS.
$$

Add the same sufficiently large nonnegative integer $H$ to all the $b_i$, obtaining $c_i=b_i+H\geq0$. The sum is unchanged because $\sum_{i\in I}a_i=0$. Let $K=\max_{i\in I}c_i$.

Apply the scaled [Brauer progression theorem](../../../../../brauer-progression-theorem.md), proved above from the permitted [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md), to obtain one-colour numbers $td$ and $a,a+d,\ldots,a+Kd$. Define

$$
x_i=a+c_i d\quad(i\in I),\qquad x_i=td\quad(i\notin I).
$$

All entries are positive and [monochromatic](../../../../../monochromatic-set.md), and

$$
\sum_i a_ix_i=a\sum_{i\in I}a_i+d\sum_{i\in I}a_ic_i+tdS=0-tSd+tSd=0.
$$

Therefore **the row is [partition regular](../../../../../partition-regular-matrix.md) exactly when some nonempty coefficient subset sums to zero**. Repetition of entries is allowed by the definition of [partition regularity](../../../../../partition-regular-matrix.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
