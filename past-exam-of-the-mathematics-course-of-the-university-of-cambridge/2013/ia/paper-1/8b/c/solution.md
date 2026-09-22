<h1 id="8b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the orthonormal right-handed basis

$$
u=\frac1{\sqrt2}(1,1,0)^T,\qquad
v=\frac1{\sqrt2}(-1,1,0)^T,\qquad w=(0,0,1)^T.
$$

Direct multiplication gives $B(r)u=u$, $B(r)v=rv+w/\sqrt2$ and $B(r)w=-v/\sqrt2+rw$. Thus the matrix in this basis is

$$
\begin{pmatrix}1&0&0\\0&r&-1/\sqrt2\\0&1/\sqrt2&r\end{pmatrix}.
$$

The last two columns are [orthogonal](../../../../../../orthogonal-vectors.md) and both have squared [norm](../../../../../../norm.md) $r^2+1/2$. Therefore $B(r)$ is an [orthogonal matrix](../../../../../../orthogonal-matrix.md) precisely when $r^2+1/2=1$, giving the unique positive value

$$
\boxed{r_0=1/\sqrt2.}
$$

Its determinant is $r_0^2+1/2=1$, so it is a proper [rotation matrix](../../../../../../rotation-matrix.md), not a reflection. The transverse block has cosine and sine both $1/\sqrt2$. Consequently

$$
\boxed{\text{axis }\{t(1,1,0):t\in\mathbb R\},\qquad\text{angle }\pi/4.}
$$

With the oriented axis $u$, the angle is positive by the right-hand rule, since $u\times v=w$. The axis also follows from the unit-[eigenvalue](../../../../../../eigenvalue.md) eigenspace. As a check, $\operatorname{tr}B(r_0)=1+\sqrt2=1+2\cos(\pi/4)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8B](../../8b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
