<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The continuous coefficients are [uniformly continuous](../../../../../../uniform-continuity.md) on a compact neighborhood of $\overline W$. For every $x_0\in\overline W$, choose a ball $B_r(x_0)\Subset U$ small enough that

$$
\|a^{ij}-a^{ij}(x_0)\|_{L^\infty(B_r(x_0))}<\frac\theta{2n}
$$

for all $i,j$. Part 4(b), with the frozen [symmetric matrix](../../../../../../symmetric-matrix.md) $A=(a^{ij}(x_0))$, then applies on this ball.

Choose a finite collection of these balls and a smooth [partition of unity](../../../../../../partition-of-unity.md) $(\eta_k)$ that sums to one near $\overline W$, with each $\eta_k$ supported in its corresponding ball. Applying part 4(b) to $\eta_k u$ gives

$$
\|D^2(\eta_k u)\|_2\leq C\|L(\eta_k u)\|_2.
$$

Since $(a^{ij})$ is symmetric, the [Leibniz rule](../../../../../../leibniz-rule.md) gives the commutator formula

$$
L(\eta_k u)
=\eta_kLu+2a^{ij}(D_i\eta_k)(D_ju)+a^{ij}(D_{ij}\eta_k)u.
$$

The coefficients and the finitely many derivatives of the [cutoff functions](../../../../../../cutoff-function.md) are bounded, so

$$
\|L(\eta_k u)\|_2
\leq C\left(\|Lu\|_{L^2(U)}+\|u\|_{H^1(U)}\right).
$$

Finally $u=\sum_k\eta_k u$ near $\overline W$. Summing the finite set of local estimates proves

$$
\boxed{\|D^2u\|_{L^2(W)}
\leq C\left(\|Lu\|_{L^2(U)}+\|u\|_{H^1(U)}\right).}
$$

This is the [coefficient-freezing interior second-derivative estimate](../../../../../../coefficient-freezing-interior-second-derivative-estimate.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
