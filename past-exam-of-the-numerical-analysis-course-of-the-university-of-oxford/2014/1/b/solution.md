<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $u=0$, any nonzero $w$, for instance the first [Cartesian basis](../../../../cartesian-basis.md) vector $e_1$, gives $H(w)u=0$ and $\alpha=0$. Suppose $u\ne0$. Choose

$$
\alpha=-\operatorname{sgn}_+(u_1)\|u\|_2,\qquad w=u-\alpha e_1,
$$

where $\operatorname{sgn}_+(r)=1$ for $r\geq0$ and $-1$ otherwise. This choice ensures $w\ne0$, including when $u$ is already on the first coordinate axis. Since $\alpha^2=u^Tu$,

$$
w^Tu=u^Tu-\alpha u_1,\qquad w^Tw=u^Tu-2\alpha u_1+\alpha^2=2(w^Tu).
$$

Therefore the [Householder reflection](../../../../householder-transformation.md) satisfies

$$
\boxed{H(w)u=u-\frac{2w(w^Tu)}{w^Tw}=u-w=\alpha e_1.}
$$

The [orthogonality](../../../../orthogonal-vectors.md) of $H(w)$, used here to check length preservation, gives $|\alpha|=\|H(w)u\|_2=\|u\|_2$. The chosen sign also avoids [catastrophic cancellation](../../../../catastrophic-cancellation.md) in $w_1=u_1-\alpha$. This is a [Householder reflection sending a vector to a coordinate axis](../../../../householder-reflection-sending-a-vector-to-a-coordinate-axis.md) with no zero-normal exception.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
