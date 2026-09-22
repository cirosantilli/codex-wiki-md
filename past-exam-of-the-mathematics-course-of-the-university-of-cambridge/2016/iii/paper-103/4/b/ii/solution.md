<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $T$ be a [standard Young tableau](../../../../../../../standard-young-tableau.md) of shape $\lambda\vdash n$, and let $\mu$ be the shape formed by its entries $1,\ldots,k$. Since [Young–Jucys–Murphy elements](../../../../../../../jucys-murphy-element.md) act by contents, the [eigenvalue](../../../../../../../eigenvalue.md) of $\xi_k$ on its [Gelfand–Tsetlin basis](../../../../../../../gelfand-tsetlin-basis.md) vector is

$$
\prod_{r=2}^k c_T(r).
$$

If $\mu$ is not a [hook partition](../../../../../../../hook-partition.md), it contains $(2,2)$, whose content is zero, so this product is zero. If $\mu=(a+1,1^b)$ with $a+b+1=k$, its nonzero contents are $1,\ldots,a$ and $-1,\ldots,-b$. Their product is independent of the order of the labels. Therefore **the [eigenvalue](../../../../../../../eigenvalue.md) is**

$$
\boxed{
\xi_kw_T=
\begin{cases}
(-1)^b a!b!\,w_T,&\mu=(a+1,1^b),\\
0,&\mu\text{ is not a hook}.
\end{cases}}
$$

The empty product at $k=1$ gives $1$. When $k=n$, $\mu=\lambda$, giving exactly the hook-versus-nonhook distinction suggested by the hint. For $k<n$, it is the intermediate shape $\mu$, rather than the final shape $\lambda$, that controls the answer.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
