<h1 id="7b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Orient the axis towards $n=(3/5,4/5,0)$ and measure positive angles by the [right-hand rule](../../../../../../right-hand-rule.md) about $n$. The [vectors](../../../../../../vector.md) $n$, $m=(-4/5,3/5,0)$ and $e_3=(0,0,1)$ form a positively oriented [orthonormal basis](../../../../../../orthonormal-basis.md), since $n\times m=e_3$. Its [change-of-basis matrix](../../../../../../change-of-basis-matrix.md) is

$$
Q=\begin{pmatrix}3/5&-4/5&0\\4/5&3/5&0\\0&0&1\end{pmatrix},\qquad Q^{-1}=Q^T.
$$

Relative to this [basis](../../../../../../basis.md), the [rotation](../../../../../../rotation-mathematics.md) fixes the first coordinate and rotates the last two. Writing $c=\cos\alpha$ and $s=\sin\alpha$, its [matrix](../../../../../../matrix.md) in the [standard basis](../../../../../../standard-basis.md) is therefore

$$
\boxed{R=Q\begin{pmatrix}1&0&0\\0&c&-s\\0&s&c\end{pmatrix}Q^T
=\begin{pmatrix}(9+16c)/25&12(1-c)/25&4s/5\\12(1-c)/25&(16+9c)/25&-3s/5\\-4s/5&3s/5&c\end{pmatrix}.}
$$

In particular $Rn=n$, $Rm=cm+se_3$, and $Re_3=-sm+ce_3$, verifying the axis and the direction of [rotation](../../../../../../rotation-mathematics.md). Reversing the chosen orientation of the axis replaces $\alpha$ by $-\alpha$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7B](../../7b.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ia](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
