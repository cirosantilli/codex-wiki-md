<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the reverse [centered polynomial birth move in reversible-jump sampling](../../../../../../../centered-polynomial-birth-move-in-reversible-jump-sampling.md), recover $z=\beta'_{k+1}$ from the current coefficient vector. Remove that highest-order coefficient and undo the intercept shift:

$$
\boxed{\beta_0=\beta'_0+c\beta'_{k+1},\qquad
\beta_i=\beta'_i\ (1\leq i\leq k),\qquad s'=s.}
$$

No auxiliary random number is drawn for this death move: the removed coefficient supplies the auxiliary value needed to reconstruct the birth move. The reverse [Jacobian determinant](../../../../../../../jacobian-determinant.md) is also one. The inverse prediction change is $-zv$, hence the residual in the lower-order model is $r=r'+zv$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
