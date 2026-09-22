<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the two arrow matrices as $(A,B)\in M_2(k)^2$. The [base change action on quiver representations](../../../../../../base-change-action-on-quiver-representations.md) sends them to $(g_2Ag_1^{-1},g_3Bg_2^{-1})$. Starting from $(I,I)$ yields precisely the pairs with both matrices invertible: given such a pair, choose $g_1=I$, $g_2=A$, $g_3=BA$. Hence

$$
\boxed{\mathcal O_X=\{(A,B):\det A\det B\ne0\}\cong\operatorname{GL}_2(k)^2}.
$$

This is a nonempty [Zariski-open subset](../../../../../../zariski-open-set.md) of the irreducible affine space $M_2(k)^2$, so its closure is the entire representation space. Its boundary in that closure is $\{\det A\det B=0\}$.

The [rank classification of a two-step linear map](../../../../../../rank-classification-of-a-two-step-linear-map.md) says an orbit is determined by $(r,s,t)=(\operatorname{rank}A,\operatorname{rank}B,\operatorname{rank}(BA))$. Indeed, the six interval multiplicities from the elementary decomposition are

$$
m_{13}=t,\quad m_{12}=r-t,\quad m_{23}=s-t,\quad m_{11}=2-r,\quad m_{22}=2-r-s+t,\quad m_{33}=2-s.
$$

They are nonnegative exactly when $0\le r,s\le2$ and $\max(0,r+s-2)\le t\le\min(r,s)$. Apart from the open orbit $(2,2,2)$, **there are nine boundary orbits**. Put $D=\operatorname{diag}(1,0)$ and $E=\operatorname{diag}(0,1)$; representatives are

$$
\begin{array}{c|c|c}
(r,s,t)&A&B\\\hline
(0,0,0)&0&0\\
(0,1,0)&0&D\\
(0,2,0)&0&I\\
(1,0,0)&D&0\\
(2,0,0)&I&0\\
(1,1,0)&D&E\\
(1,1,1)&D&D\\
(1,2,1)&D&I\\
(2,1,1)&I&D
\end{array}
$$

The two rank-one/rank-one cases differ by whether $\operatorname{im}A\subseteq\ker B$; the individual arrow ranks alone do not distinguish them.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
