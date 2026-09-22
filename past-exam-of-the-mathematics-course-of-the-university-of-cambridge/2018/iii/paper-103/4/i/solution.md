<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We use the [abacus divisible-hook correspondence](../../../../../../hooks-divisible-by-the-abacus-modulus.md) in its multiset form: the [hook lengths](../../../../../../hook-length.md) of $\lambda$ that are divisible by $p$, divided by $p$, form exactly the disjoint union of the [multisets](../../../../../../multiset.md) of [hook lengths](../../../../../../hook-length.md) of the components of its [quotient of a partition](../../../../../../quotient-of-a-partition.md) for modulus $p$.

Iterating this correspondence gives, for every $r\geq1$,

$$
\{h/p^r:h\in\mathcal H(\lambda),\ p^r\mid h\}
=\bigsqcup_{\eta\in T^Q(\lambda)_r}\mathcal H(\eta)
$$

as [multisets](../../../../../../multiset.md). Each [Young diagram](../../../../../../young-diagram.md) has one hook for every cell, so the [cardinality](../../../../../../cardinality.md) of the right-hand side is $|T^Q(\lambda)_r|$, the sum of the component sizes.

For any positive integer $h$, its [P-adic valuation](../../../../../../p-adic-valuation.md) is the number of positive $r$ for which $p^r\mid h$. Summing this identity over hooks and interchanging the finite sums proves

$$
\begin{aligned}
\nu_p\!\left(\prod_{h\in\mathcal H(\lambda)}h\right)
&=\sum_{h\in\mathcal H(\lambda)}\sum_{r\geq1}\mathbf1_{p^r\mid h}\\
&=\sum_{r\geq1}|T^Q(\lambda)_r|.
\end{aligned}
$$

Thus

$$
\boxed{\nu_p\!\left(\prod_{h\in\mathcal H(\lambda)}h\right)=\sum_{r\geq1}|T^Q(\lambda)_r|.}
$$

The sums are finite because hook lengths are bounded by $|\lambda|$, and the total size at each level of the [quotient tower of a partition](../../../../../../quotient-tower-of-a-partition.md) decreases by at least a factor $p$ until it reaches zero.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
