<h1 id="3k/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A square-free monomial in $d$ variables of degree $j\leq d-1$ evaluates to one at exactly $2^{d-j}$ points of $\mathbb F_2^d$, an even number. Since parity of [Hamming weight](../../../../../../../hamming-weight.md) is a linear functional over $\mathbb F_2$, every sum of such evaluation words also has even weight. Hence every word in $\operatorname{RM}(d,d-1)$ has even weight.

If $f$ and $g$ have degrees at most $r$ and $d-r-1$, then $fg$ has degree at most $d-1$. The binary inner product of their evaluation words is the parity of the weight of the evaluation of $fg$, and is therefore zero. Thus

$$
\operatorname{RM}(d,d-r-1)
\subseteq\operatorname{RM}(d,r)^\perp.
$$

Finally, binomial symmetry gives

$$
\dim\operatorname{RM}(d,r)
+\dim\operatorname{RM}(d,d-r-1)=2^d,
$$

so the inclusion has equal dimensions and

$$
\boxed{
\operatorname{RM}(d,r)^\perp
=\operatorname{RM}(d,d-r-1)
}.
$$

This is the [Dual of a Reed-Muller code](../../../../../../../dual-of-a-reed-muller-code.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3K](../../../3k.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
