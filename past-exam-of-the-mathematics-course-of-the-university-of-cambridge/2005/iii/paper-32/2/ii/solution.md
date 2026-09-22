<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The squares in $\mathbb F_5$ are $0,1,4$. The following table counts affine solutions at each $x$, with one point at infinity to be added:

$$
\begin{array}{c|ccccc}
x&0&1&2&3&4\\\hline
x^3-x&0&0&1&4&0\\
\#\{y:y^2=x^3-x\}&1&1&2&2&1\\
x^3-x+1&1&1&2&0&1\\
\#\{y:y^2=x^3-x+1\}&2&2&0&1&2
\end{array}
$$

Hence $\#E_1(\mathbb F_5)=\#E_2(\mathbb F_5)=8$. In characteristic five, a finite point has order two precisely when $y=0$. The first cubic has three roots $0,1,4$, giving four elements killed by two, including $O$. The second cubic has only the root $3$, giving two elements killed by two. An isomorphism of [groups](../../../../../../group-split.md) would preserve these counts, so the [groups](../../../../../../group-split.md) are not isomorphic.

More precisely $(2,1)\in E_1$ doubles to $(0,0)$ and has order four; the independent two-torsion point $(1,0)$ gives $C_4\times C_2$. On $E_2$, the point $(0,1)$ doubles to $(4,1)$, which doubles to $(3,0)$; it therefore has order eight. Thus the [eight-point isogenous elliptic curves over F5](../../../../../../eight-point-isogenous-elliptic-curves-over-f5.md) have point [groups](../../../../../../group-split.md)

$$
\boxed{E_1(\mathbb F_5)\cong C_4\times C_2,\qquad E_2(\mathbb F_5)\cong C_8.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
