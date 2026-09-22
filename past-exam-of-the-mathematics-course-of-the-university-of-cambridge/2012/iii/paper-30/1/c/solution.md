<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Count [partially directed self-avoiding walks](../../../../../../partially-directed-self-avoiding-walk.md) using north, east and west steps. Within one horizontal level, a [self-avoiding walk](../../../../../../self-avoiding-walk.md) must move consistently east or consistently west. It can change horizontal direction only after a north step. Conversely, these rules guarantee self-avoidance: every visited horizontal level is new, and its horizontal run is monotone.

Let $a_n$ count these walks, including $a_0=1$. A horizontal run has [generating function](../../../../../../generating-function.md)

$$
R(z)=1+2\sum_{\ell\ge1}z^\ell=\frac{1+z}{1-z}.
$$

Every walk decomposes uniquely into an initial horizontal run followed by zero or more pairs consisting of a north step and a horizontal run. Therefore the [generating function](../../../../../../generating-function.md) is

$$
A(z)=\sum_{n\ge0}a_nz^n=\frac{R(z)}{1-zR(z)}
=\frac{1+z}{1-2z-z^2}.
$$

Comparing coefficients yields $a_0=1$, $a_1=3$, and $a_n=2a_{n-1}+a_{n-2}$ for $n\ge2$. Solving this [linear recurrence relation](../../../../../../linear-recurrence-relation.md) gives

$$
a_n=\frac{(1+\sqrt2)^{n+1}+(1-\sqrt2)^{n+1}}2.
$$

These are a subset of all [self-avoiding walks](../../../../../../self-avoiding-walk.md), so $c_n\ge a_n$ and

$$
\boxed{\kappa\ge\lim_{n\to\infty}a_n^{1/n}=1+\sqrt2>2.}
$$

Allowing either horizontal direction at successive heights gives the strict gain over the north-east-only family.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
