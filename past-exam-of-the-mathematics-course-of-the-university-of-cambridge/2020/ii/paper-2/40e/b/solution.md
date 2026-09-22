<h1 id="40e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an iterate $x_m$, the [Conjugate gradient method](../../../../../../conjugate-gradient-method.md) residual is

$$
\boxed{r_m=b-Ax_m}.
$$

Two fundamental properties are the [Conjugate-gradient residual orthogonality](../../../../../../conjugate-gradient-residual-orthogonality.md) conditions

$$
r_m\perp\mathcal K_m(A,r_0),
\qquad
r_m\in\mathcal K_{m+1}(A,r_0).
$$

Equivalently, the residuals generated before convergence are mutually orthogonal and span the successive Krylov spaces.

Since $A$ has only $s$ distinct eigenvalues, its minimal polynomial has degree at most $s$. Consequently

$$
\mathcal K_{s+1}(A,r_0)=\mathcal K_s(A,r_0).
$$

The two properties then put $r_s$ both inside and orthogonal to $\mathcal K_s(A,r_0)$, so $r_s=0$. Hence $Ax_s=b$, and

$$
\boxed{\text{CG terminates after at most }s\text{ iterations}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40E](../../40e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
