<h1 id="21f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $f\in\sqrt I$, a power $f^m$ vanishes at every point of $Z(I)$, so $f$ itself vanishes there. This gives $\sqrt I\subseteq I(Z(I))$.

For the reverse inclusion, take $f$ vanishing on $Z(I)$ and use the [Rabinowitsch trick](../../../../../../rabinowitsch-trick.md). In $k[x_1,\ldots,x_n,t]$ form $J=(I,1-tf)$. A common zero would have $x\in Z(I)$, whence $f(x)=0$ and $1-tf(x)=1$, a contradiction. The assumed [Weak Hilbert Nullstellensatz](../../../../../../weak-hilbert-nullstellensatz.md) gives $J=(1)$. Thus there is a finite expression

$$
1=\sum_ja_j(x,t)i_j(x)+b(x,t)(1-tf(x)),\qquad i_j\in I.
$$

If $f=0$ the conclusion is immediate. Otherwise substitute $t=f^{-1}$ in the localized [polynomial](../../../../../../polynomial-split.md) ring. The last term vanishes, and clearing a sufficiently high power of $f$ gives $f^N\in I$. Hence $f\in\sqrt I$, proving the [Strong Hilbert Nullstellensatz](../../../../../../strong-hilbert-nullstellensatz.md):

$$
\boxed{I(Z(I))=\sqrt I.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [21F](../../21f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
