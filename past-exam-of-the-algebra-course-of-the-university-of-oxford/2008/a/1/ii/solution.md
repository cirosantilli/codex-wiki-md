<h1 id="a/1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**A [noncommutative](../../../../../noncommutativity.md) [algebra](../../../../../algebra-split.md) may have a [commutative](../../../../../commutativity.md) quotient:** take $A=K\times M_2(K)$, $B=K$, and $\varphi(\lambda,M)=\lambda$. This is a surjective unital homomorphism. Neither requested change of commutativity can occur for an isomorphism, since an isomorphism transfers the identity $ab=ba$ in both directions.

For the matrix classifications, write $E_{ij}$ for a [matrix unit](../../../../../matrix-unit.md) and $N=E_{12}+E_{23}$. Then $N^2=E_{13}$ and $N^3=0$. The complete square-zero sets and commutativity results are

$$
\begin{array}{c|c|c}
 &\text{commutative?}&\{\alpha:\alpha^2=0\}\\\hline
A_1&\text{yes}&\{0\}\\
A_2&\text{yes}&KE_{12}+KE_{13}\\
A_3&\text{yes}&KE_{13}\\
A_4&\text{no}&KE_{12}\\
A_5&\text{yes}&KE_{13}+KE_{23}.
\end{array}
$$

Indeed $A_1$ is diagonal. In $A_2$ and $A_5$ the two off-diagonal generators have all products zero, so multiplication has the form $(x,u)(x',u')=(xx',xu'+x'u)$. The diagonal entries of a square force $x=0$, after which the off-diagonal part squares to zero. In $A_3=K[N]$, a square-zero element first has scalar coefficient zero and then $(yN+zN^2)^2=y^2N^2$, forcing $y=0$. This argument works also in characteristic two. In $A_4$, a square first forces both diagonal parameters to vanish, leaving precisely $KE_{12}$. Noncommutativity follows from $E_{22}E_{12}=0$ but $E_{12}E_{22}=E_{12}$.

The coordinate map $xI+yE_{12}+zE_{13}\mapsto xI+yE_{13}+zE_{23}$ is an isomorphism $A_2\to A_5$, by the common multiplication formula. Every other pair is nonisomorphic: $A_4$ is the only [noncommutative](../../../../../noncommutativity.md) member, and among the [commutative](../../../../../commutativity.md) members the dimensions of the square-zero sets are respectively zero, two, one, and two. These sets are vector spaces in these examples, and an [algebra isomorphism](../../../../../algebra-isomorphism.md) must carry one onto the other. Thus **the only distinct isomorphic pair is $A_2\cong A_5$**.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the algebra course of the University of Oxford](../../../../split.md)
6. [Algebra course of the University of Oxford](../../../../../algebra-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
