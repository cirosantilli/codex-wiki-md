<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\overline\nabla f$ and $\overline{\operatorname{Hess}}f$ be the ambient gradient and Hessian. The [Laplacian of a restricted ambient function](../../../../../../laplacian-of-a-restricted-ambient-function.md) is

$$
\Delta_M(f|_M)
=\operatorname{tr}_{TM}(\overline{\operatorname{Hess}}f)
+\langle\overline\nabla f,\mathbf H\rangle.
$$

To prove it, choose a local orthonormal tangent frame $e_1,\ldots,e_n$ with $\nabla^M_{e_i}e_j=0$ at the point under consideration. There,

$$
\begin{aligned}
\Delta_M(f|_M)
&=\sum_i e_i(e_i f)\\
&=\sum_i\left(\overline{\operatorname{Hess}}f(e_i,e_i)
+\langle\overline\nabla f,\overline\nabla_{e_i}e_i\rangle\right)\\
&=\sum_i\overline{\operatorname{Hess}}f(e_i,e_i)
+\left\langle\overline\nabla f,\sum_iA(e_i,e_i)\right\rangle.
\end{aligned}
$$

Both sides are intrinsic scalars, so the pointwise calculation proves the formula everywhere.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
