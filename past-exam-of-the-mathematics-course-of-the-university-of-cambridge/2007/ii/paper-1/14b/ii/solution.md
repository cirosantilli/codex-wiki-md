<h1 id="14b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Contract the loops in the [Pochhammer contour](../../../../../../pochhammer-contour.md) onto the interval $(0,1)$. When $\operatorname{Re}z,\operatorname{Re}b>0$, the small-circle contributions tend to zero. The two clockwise circuits change the branches by $e^{-2\pi ib}$ and $e^{-2\pi iz}$, and the return circuits undo them. The four interval contributions sum to

$$
J(z)=(1-e^{-2\pi iz})(1-e^{-2\pi ib})\int_0^1t^{z-1}(1-t)^{b-1}\,dt.
$$

Using the [Beta function](../../../../../../beta-function.md) and $1-e^{-2\pi iu}=2ie^{-\pi iu}\sin(\pi u)$ gives

$$
\boxed{J(z)=-4e^{-\pi i(z+b)}\sin(\pi z)\sin(\pi b)B(z,b).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14B](../../14b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
