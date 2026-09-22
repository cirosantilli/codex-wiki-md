<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md), the [moment-generating function](../../../../../../moment-generating-function.md) is

$$
M(\tau)=\frac{e^\tau+e^{-\tau}}2=\cosh\tau.
$$

For a given $\alpha>0$, choose the unique $\tau>0$ satisfying $\cosh\tau=e^\alpha$. The transform in part (d) becomes $\mathbb E e^{-\alpha T}=e^{-b\tau}$. To express this in terms of $\alpha$, put $r=e^{-\tau}\in(0,1)$. The equation $(r+r^{-1})/2=e^\alpha$ gives $r^2-2e^\alpha r+1=0$. Its smaller root is the one in $(0,1)$, so

$$
\boxed{\mathbb E[e^{-\alpha T}]
=\left(e^\alpha-\sqrt{e^{2\alpha}-1}\right)^b
=\left(\frac{e^{-\alpha}}{1+\sqrt{1-e^{-2\alpha}}}\right)^b.}
$$

The second expression follows by rationalizing the first root. As $\alpha\downarrow0$ the transform tends to one, consistent with the almost-sure finiteness proved in part (c).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
