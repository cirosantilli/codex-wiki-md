<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In the notation of part (i), the tensor [raising operator](../../../../../../../raising-operator.md) and [lowering operator](../../../../../../../lowering-operator.md) act by

$$
eA_k=kA_{k-1},\quad eB_k=A_k+kB_{k-1},\qquad fA_k=B_k+(3-k)A_{k+1},\quad fB_k=(3-k)B_{k+1},
$$

with terms beyond the stated index range omitted. Both $v_4=A_0$ and $v_2=B_0-A_1$ are killed by $e$, and have respective weights four and two. They are the desired [highest-weight vectors](../../../../../../../highest-weight-vector.md).

For $v_4$, successive lowering gives

$$
fv_4=3A_1+B_0,\quad f^2v_4=6(A_2+B_1),\quad f^3v_4=6(A_3+3B_2),\quad f^4v_4=24B_3,\quad f^5v_4=0.
$$

Thus a [basis](../../../../../../../basis.md) of the five-dimensional summand, in descending weight order, is

$$
\boxed{L(4)=\operatorname{span}\{A_0,\ 3A_1+B_0,\ A_2+B_1,\ A_3+3B_2,\ B_3\},\quad v_4=A_0.}
$$

For $v_2$, the successive vectors are $fv_2=2(B_1-A_2)$, $f^2v_2=2(B_2-A_3)$ and $f^3v_2=0$. Hence

$$
\boxed{L(2)=\operatorname{span}\{B_0-A_1,\ B_1-A_2,\ B_2-A_3\},\quad v_2=B_0-A_1.}
$$

These spans are invariant under $h,e,f$. The [sl2 highest-weight lowering formula](../../../../../../../sl2-highest-weight-lowering-formula.md) gives $ef^rv_n=r(n-r+1)f^{r-1}v_n$, so all interior raising coefficients in either chain are nonzero. Any nonzero submodule therefore contains the highest vector and then the whole chain; each span is irreducible.

At the shared weights $2,0,-2$, the two displayed summand vectors are independent: their coefficient determinants in the original weight bases are $4,2,4$. At weights $4,-4$ only the five-dimensional summand occurs. Consequently the eight displayed vectors form a basis of $U$, proving that these are complementary submodules, not only modules with the right dimensions.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
