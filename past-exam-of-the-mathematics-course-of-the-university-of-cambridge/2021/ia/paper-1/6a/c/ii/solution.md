<h1 id="6a/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Each entry of $\operatorname{adj}(M-tI)$ is, up to sign, the determinant of an $(n-1)\times(n-1)$ minor whose entries are affine polynomials in $t$. The [Leibniz formula for determinants](../../../../../../../leibniz-formula-for-determinants.md) therefore makes each adjugate entry a polynomial in $t$ of degree at most $n-1$.

For arbitrary $A,B$, choose positive sequences $s_j,t_j\to0$ for which $A-s_jI$ and $B-t_jI$ are nonsingular. The nonsingular identity from part (b) applies to their product:

$$
\operatorname{adj}((A-s_jI)(B-t_jI))
=\operatorname{adj}(B-t_jI)\operatorname{adj}(A-s_jI).
$$

Every entry is a polynomial, hence continuous, in the matrix entries. Letting $j\to\infty$ proves

$$
\boxed{\operatorname{adj}(AB)
=\operatorname{adj}(B)\operatorname{adj}(A)}
$$

for all square matrices.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6A](../../../6a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
