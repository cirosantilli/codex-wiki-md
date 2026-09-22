<h1 id="6d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**True.** Use the [odd-dimensional orthogonal determinant splitting](../../../../../../odd-dimensional-orthogonal-determinant-splitting.md):

$$
\boxed{\Phi:O(3)\to SO(3),\qquad \Phi(A)=(\det A)A.}
$$

Scalar matrices commute with every matrix, so $\Phi(AB)=\Phi(A)\Phi(B)$. Its output is orthogonal and

$$
\det\Phi(A)=(\det A)^3\det A=(\det A)^4=1.
$$

Every $B\in SO(3)$ satisfies $\Phi(B)=B$, proving surjectivity. The equation $\Phi(A)=I$ forces $A=(\det A)I$, whence

$$
\boxed{\ker\Phi=\{I,-I\},\qquad |\ker\Phi|=2.}
$$

In odd dimension $-I$ has [determinant](../../../../../../determinant.md) $-1$, which is the sign needed in this construction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
