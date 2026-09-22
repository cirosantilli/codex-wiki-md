<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A rational matrix is a [partition regular matrix](../../../../../partition-regular-matrix.md) when every finite coloring of the positive integers admits a monochromatic positive vector in its kernel. Its columns have the [columns property](../../../../../columns-property.md) if their indices can be partitioned into ordered nonempty blocks $B_1,\ldots,B_s$ such that the columns in $B_1$ sum to zero and, for $j>1$, the sum over $B_j$ lies in the rational linear span of the columns in the earlier blocks. [Rado's theorem](../../../../../rado-s-theorem.md) states that a rational matrix is partition regular if and only if its columns have this property.

For one equation, clear denominators and write

$$
c_1x_1+\cdots+c_nx_n=0,
\qquad c_i\in\mathbb Z\setminus\{0\}.
$$

The one-row columns property is equivalent to the existence of a nonempty $I\subseteq[n]$ with

$$
\sum_{i\in I}c_i=0.
$$

First suppose such an $I$ exists. Choose $i_0\in I$, put $c=|c_{i_0}|$, $C=\sum_{j\notin I}c_j$, and choose $p\geq|C|$. The [monochromatic m-p-c set theorem](../../../../../monochromatic-m-p-c-set-theorem.md), whose finite induction proof uses the [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md), gives positive $z_1,z_2$ for which all numbers

$$
cz_1+\lambda z_2\quad(|\lambda|\leq p),
\qquad cz_2
$$

are positive and have one color. Set

$$
x_i=cz_1\quad(i\in I\setminus\{i_0\}),
\qquad
x_{i_0}=cz_1-\frac{Cc}{c_{i_0}}z_2,
\qquad
x_j=cz_2\quad(j\notin I).
$$

The middle coefficient is the integer $-C\operatorname{sgn}(c_{i_0})$, of absolute value at most $p$, so all the $x_i$ belong to the monochromatic set. Their $z_1$ contribution vanishes because the coefficients over $I$ sum to zero, and their $z_2$ contribution is

$$
c_{i_0}\left(-\frac{Cc}{c_{i_0}}\right)+Cc=0.
$$

Thus the equation is partition regular.

Conversely, suppose no nonempty subset of the coefficients sums to zero. Choose a [prime number](../../../../../prime-number.md) $p$ that divides none of the finitely many nonzero subset sums. Color each positive integer by its [last nonzero digit coloring](../../../../../last-nonzero-digit-coloring.md) in base $p$. If a monochromatic solution existed, let $v$ be the smallest [P-adic valuation](../../../../../p-adic-valuation.md) among its coordinates and let $I$ index the coordinates of valuation $v$. After division by $p^v$ and reduction modulo $p$, all $x_i$ with $i\in I$ have the same nonzero last digit $r$, while the other terms vanish. The equation would give

$$
r\sum_{i\in I}c_i\equiv0\pmod p,
$$

contrary to the choice of $p$. This proves the [Rado theorem for one equation](../../../../../rado-theorem-for-one-equation.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
