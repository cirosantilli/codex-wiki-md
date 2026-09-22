<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $e_1,\ldots,e_m$ be the standard basis of $\mathbb F_2^m$ and take

$$
A_m=\{0,e_1,\ldots,e_m\}.
$$

Its [sumset](../../../../../../sumset.md) consists of zero, the $m$ basis vectors, and the $\binom m2$ sums of two distinct basis vectors. Thus

$$
K_m=\frac{|A_m+A_m|}{|A_m|}
=\frac{1+m+\binom m2}{m+1}
=\frac m2+\frac1{m+1}.
$$

If a coset $x+H$ contains $A_m$, then every difference of two elements of $A_m$ lies in $H$. In particular every $e_i$ lies in $H$, so $H=\mathbb F_2^m$ and

$$
\frac{|H|}{|A_m|}=\frac{2^m}{m+1}.
$$

Since $m=2K_m+O(1)$, this ratio is eventually much larger than $K_m^{-1}2^{K_m}$. Hence no bound valid for all $K$ can replace the factor in part c by a function smaller than $K^{-1}2^K$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
