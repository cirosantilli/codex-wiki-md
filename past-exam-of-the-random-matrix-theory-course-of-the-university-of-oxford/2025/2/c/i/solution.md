<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [correlation functions of a point process](../../../../../correlation-function-of-a-point-process.md) use factorial normalization:

$$
R_3^{(k)}(x_1,\ldots,x_k)
=\frac{3!}{(3-k)!}\int_{\mathbb R^{3-k}}
\rho_3(x_1,x_2,x_3)\,dx_{k+1}\cdots dx_3.
$$

Start with $\rho_3=D_3/6$. By [Gaudin's lemma](../../../../../projection-kernel-determinant-integration.md), integrating $D_3$ once gives $D_2$, and integrating $D_2$ once gives $2D_1$. The factorial factors cancel, so the [eigenvalues](../../../../../eigenvalue.md) form a [determinantal point process](../../../../../determinantal-point-process.md) with

$$
\boxed{R_3^{(1)}(x)=\widetilde K_3(x,x),}
$$

and

$$
\boxed{R_3^{(2)}(x,y)
=\det\begin{pmatrix}
\widetilde K_3(x,x)&\widetilde K_3(x,y)\\
\widetilde K_3(y,x)&\widetilde K_3(y,y)
\end{pmatrix}
=\widetilde K_3(x,x)\widetilde K_3(y,y)-\widetilde K_3(x,y)^2.}
$$

The last equality uses the real symmetry of this kernel. In particular, $\int R_3^{(1)}=3$ and $\iint R_3^{(2)}=6$, as required for three points and six ordered pairs of distinct points.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
