<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put

$$
q_r=|TQ_p(\lambda)_r|,
\qquad
c_r=|TC_p(\lambda)_r|.
$$

The defining relation between the [quotient tower of a partition](../../../../../../quotient-tower-of-a-partition.md) and the [core tower of a partition](../../../../../../core-tower-of-a-partition.md) is

$$
q_r=c_r+pq_{r+1},
\qquad q_0=n.
$$

Summing the resulting telescoping identities gives

$$
\sum_{r\geq0}c_r=n-(p-1)\sum_{r\geq1}q_r.
$$

By the [Hook-length formula](../../../../../../hook-length-formula.md),

$$
v_p(\chi^\lambda(1))=v_p(n!)-\sum_{x\in Y(\lambda)}v_p(h_x).
$$

The [abacus divisible-hook correspondence](../../../../../../hooks-divisible-by-the-abacus-modulus.md) says that the number of hooks divisible by $p^r$ is $q_r$, so

$$
\sum_xv_p(h_x)=\sum_{r\geq1}q_r.
$$

If $d_p(n)=\sum_r\alpha_r$, the digit-sum form of the [Legendre formula](../../../../../../legendre-s-formula.md) is

$$
v_p(n!)=\frac{n-d_p(n)}{p-1}.
$$

Combining the three displayed identities proves the [P-adic valuation of a symmetric-group character degree from the core tower](../../../../../../p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower.md) formula

$$
\boxed{
v_p(\chi^\lambda(1))
=\frac{\sum_{r\geq0}|TC_p(\lambda)_r|-\sum_{r\geq0}\alpha_r}{p-1}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 160](../../../paper-160-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
