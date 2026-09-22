<h1 id="6d/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $U_t=\begin{pmatrix}1&t\\0&1\end{pmatrix}$ and $D_r=\operatorname{diag}(r,r^{-1})$, direct multiplication gives $D_rU_1D_r^{-1}=U_{r^2}$. In $\mathbb F_{11}$, $5^2=3$ and $5^{-1}=9$, so

$$
\boxed{\begin{pmatrix}5&0\\0&9\end{pmatrix}A\begin{pmatrix}5&0\\0&9\end{pmatrix}^{-1}=B\quad\text{in }\mathrm{SL}_2(11).}
$$

To rule out all conjugators when $p=5$, suppose $PAP^{-1}=B$ and write $P=\begin{pmatrix}r&s\\t&u\end{pmatrix}$. Comparing $PA=BP$ gives $t=0$ and $r=3u$. Its [determinant](../../../../../../../determinant.md) condition is $ru=1$, so $r^2=3$. The nonzero squares modulo five are $1$ and $4$, and therefore no such $P$ exists. **The two matrices are not conjugate in $\mathrm{SL}_2(5)$.** This is the square-class obstruction in [unipotent conjugacy in SL2 over a finite field](../../../../../../../unipotent-conjugacy-in-sl2-over-a-finite-field.md); checking only diagonal conjugators would not by itself exclude every possible conjugator.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6D](../../../6d.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
