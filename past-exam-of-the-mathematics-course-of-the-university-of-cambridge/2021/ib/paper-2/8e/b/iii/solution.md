<h1 id="8e/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If $\alpha\ne\beta$, the operator $f-\beta I$ is invertible on $W_{\alpha,n}$. Indeed, there it equals

$$
(\alpha-\beta)I+N,
\qquad N=f-\alpha I,\qquad N^n=0,
$$

whose inverse is the finite [geometric series](../../../../../../../geometric-series.md)

$$
\frac1{\alpha-\beta}
\sum_{k=0}^{n-1}
\left(-\frac{N}{\alpha-\beta}\right)^k.
$$

Now use induction on $d$. If $\sum_{i=1}^dv_i=0$, apply $(f-\alpha_dI)^n$. The $v_d$ term vanishes, while every transformed vector

$$
(f-\alpha_dI)^nv_i,\qquad i<d,
$$

is nonzero by the invertibility just proved and still lies in $W_{\alpha_i,n}$. The induction hypothesis rules out the resulting relation. Allowing scalar coefficients, and omitting zero terms, gives the same argument. Hence the [generalized eigenspaces for distinct eigenvalues form a direct sum](../../../../../../../generalized-eigenspaces-for-distinct-eigenvalues-form-a-direct-sum.md), so $v_1,\ldots,v_d$ are linearly independent.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8E](../../../8e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
