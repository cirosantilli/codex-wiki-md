<h1 id="10/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $B=\left(\begin{smallmatrix}0&b\\c&0\end{smallmatrix}\right)$ be the lower block. Then

$$
B^2=bcI_2,\qquad T(a)^2=\operatorname{diag}(1,bc,bc),\qquad T(a)^4=\operatorname{diag}(1,(bc)^2,(bc)^2).
$$

The defining relation $a^4=I$ requires $T(a)^4=I_3$, so for real constants $bc=\pm1$. Both possibilities ensure invertibility.

If $bc=-1$, the generator matrix has order four, because its square is not the identity while its fourth power is. Its four powers are distinct, giving a [faithful representation](../../../../../faithful-representation.md). If $bc=1$, its square is the identity but it is not itself the identity; its lower diagonal entries are zero. The image then has order two and the [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is $\{I,a^2\}$. Thus the [faithfulness criterion for a block representation of the cyclic group of order four](../../../../../faithfulness-criterion-for-a-block-representation-of-the-cyclic-group-of-order-four.md) gives

$$
\boxed{\text{faithful exactly when }bc=-1;\qquad\text{unfaithful representation exactly when }bc=1.}
$$

Other parameter values give no representation of $Z_4$, not additional unfaithful cases; $bc=0$ also makes the assigned matrix singular. No orthogonality of these matrices was required.

For the final construction take

$$
\boxed{D(a)=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad D(a^r)=\begin{pmatrix}1&0\\0&(-1)^r\end{pmatrix}.}
$$

Multiplication adds exponents, so $D(a^r)D(a^s)=D(a^{r+s})$ and $D(a)^4=I_2$. The representing matrix is the identity exactly for even exponents. Therefore this is a two-dimensional representation with kernel **$\{I,a^2\}$**, as required. It factors through the quotient cyclic group of order two.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
