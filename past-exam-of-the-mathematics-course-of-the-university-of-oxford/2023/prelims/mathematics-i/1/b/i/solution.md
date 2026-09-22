<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

If $A$ is a [strictly upper triangular matrix](../../../../../../../strictly-upper-triangular-matrix.md), then $A_{ij}=0$ unless $j-i\ge1$. We prove by [mathematical induction](../../../../../../../mathematical-induction.md) that

$$
(A^k)_{ij}=0\qquad\text{whenever }j-i<k.
$$

The assertion for $k=1$ is the definition. In the [matrix multiplication](../../../../../../../matrix-multiplication.md) formula

$$
(A^{k+1})_{ij}=\sum_{\ell=1}^n(A^k)_{i\ell}A_{\ell j},
$$

a nonzero summand would require $\ell-i\ge k$ and $j-\ell\ge1$, hence $j-i\ge k+1$. This proves the induction step. Since $j-i\le n-1$ for all entries, $\boxed{A^n=0}$. In particular, every [strictly upper triangular matrix](../../../../../../../strictly-upper-triangular-matrix.md) is a [nilpotent matrix](../../../../../../../nilpotent-matrix.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [b](../../b.md)
3. [1](../../../1.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
