<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Let $J=\begin{pmatrix}0&1\\-1&0\end{pmatrix}$. Since $J^2=-I_2$ and $J^4=I_2$, its powers define the [representation](../../../../group-representation.md) of the cyclic group of order four:

$$
\boxed{\rho(1)=I_2,\qquad\rho(-1)=-I_2,\qquad\rho(-i)=-J.}
$$

For the [quaternion group](../../../../quaternion-group.md), denote the three displayed complex [matrices](../../../../matrix.md) by $A,B,C$. Direct multiplication gives $A^2=B^2=C^2=-I_2$, $AB=C$, $BA=-C$, and $ABC=-I_2$. Together with the images of $\pm1$, these are exactly the quaternion multiplication relations, proving that the assignment defines a [group homomorphism](../../../../group-homomorphism.md) into $\operatorname{GL}(2,\mathbb C)$.

Use the [realification of a complex representation](../../../../realification-of-a-complex-representation.md): for $M=X+iY$, define $\mathcal R(M)=\begin{pmatrix}X&-Y\\Y&X\end{pmatrix}$. It acts on grouped real and imaginary coordinates and satisfies $\mathcal R(MN)=\mathcal R(M)\mathcal R(N)$. The explicit generators are

$$
\boxed{D(i)=\begin{pmatrix}0&0&0&-1\\0&0&-1&0\\0&1&0&0\\1&0&0&0\end{pmatrix},\quad
D(j)=\begin{pmatrix}0&0&-1&0\\0&0&0&1\\1&0&0&0\\0&-1&0&0\end{pmatrix},\quad
D(k)=\begin{pmatrix}0&1&0&0\\-1&0&0&0\\0&0&0&1\\0&0&-1&0\end{pmatrix}.}
$$

Set $D(1)=I_4$ and $D(-q)=-D(q)$ to specify all eight elements.

For an invertible real $S$, the [equivalent representation](../../../../equivalence-of-group-representations.md) $\widetilde D(q)=SD(q)S^{-1}$ obeys $\widetilde D(q_1)\widetilde D(q_2)=SD(q_1q_2)S^{-1}=\widetilde D(q_1q_2)$. The [trace](../../../../matrix-trace.md) is invariant under similarity, so their [characters](../../../../character-of-a-representation.md) agree. Explicitly,

$$
\boxed{\chi(1)=4,\qquad\chi(-1)=-4,\qquad\chi(\pm i)=\chi(\pm j)=\chi(\pm k)=0.}
$$

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
