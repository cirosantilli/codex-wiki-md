<h1 id="6e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write both nonnegative [integers](../../../../../../integer.md) $n,k$ in [base-p expansions](../../../../../../base-p-expansion.md), padding with zero digits to a common length $L$. By the preceding polynomial identity,

$$
(1+x)^n=\prod_{i=0}^L\left((1+x)^{p^i}\right)^{n_i}\equiv\prod_{i=0}^L(1+x^{p^i})^{n_i}\pmod p.
$$

Expanding the last product with the [binomial theorem](../../../../../../binomial-theorem.md), each term is obtained by choosing an [integer](../../../../../../integer.md) $j_i$ with $0\le j_i\le n_i<p$. Its exponent is $\sum_i j_ip^i$ and its coefficient is $\prod_i\binom{n_i}{j_i}$. Uniqueness of [base-p expansions](../../../../../../base-p-expansion.md) says that the only way this exponent can equal $k$ is to choose $j_i=k_i$ for every $i$.

If some $k_i>n_i$, no such term exists and the coefficient is zero. Otherwise its coefficient is precisely the product below. Comparing the coefficient of $x^k$ proves [Lucas theorem](../../../../../../lucas-s-theorem.md):

$$
\boxed{\binom nk\equiv\prod_{i=0}^L\binom{n_i}{k_i}\pmod p,}
$$

with the convention $\binom ab=0$ for $b>a$. This also covers $k>n$, and padding either expansion by further zero digits multiplies the product only by $\binom00=1$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
