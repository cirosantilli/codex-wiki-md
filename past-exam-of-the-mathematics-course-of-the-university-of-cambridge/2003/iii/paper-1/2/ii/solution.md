<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Killing form](../../../../../../killing-form.md) is the bilinear form

$$
\boxed{B(X,Y)=\operatorname{tr}(\operatorname{ad}X\operatorname{ad}Y),\qquad\operatorname{ad}X(Z)=[X,Z].}
$$

The [Adjoint representation](../../../../../../adjoint-representation-of-a-lie-algebra.md) is linear, giving bilinearity, and the cyclic property of [trace](../../../../../../matrix-trace.md) gives symmetry. To prove invariance, abbreviate the adjoint matrices of $X,Y,Z$ by $A_X,A_Y,A_Z$. The [Jacobi identity](../../../../../../jacobi-identity.md) gives $A_{[X,Y]}=[A_X,A_Y]$, and cyclic trace then gives

$$
\begin{aligned}
B([X,Y],Z)&=\operatorname{tr}\bigl((A_XA_Y-A_YA_X)A_Z\bigr)\\
&=\operatorname{tr}\bigl(A_X(A_YA_Z-A_ZA_Y)\bigr)=B(X,[Y,Z]).
\end{aligned}
$$

Thus $\boxed{B([X,Y],Z)=B(X,[Y,Z])}$, equivalently $B([X,Y],Z)+B(Y,[X,Z])=0$. This is infinitesimal invariance of the [Killing form](../../../../../../killing-form.md), with no choice of basis affecting the trace.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
