# Underdetermined minimum-norm example

↑ **Parent:** [Moore-Penrose inverse](moore-penrose-inverse.md)

Now take one equation for two unknowns:

$$
A=\begin{pmatrix}1&2\end{pmatrix},
\qquad b=3.
$$

The [linear system](system-of-linear-equations.md) $x_1+2x_2=3$ has an entire [affine line](affine-line.md) of exact solutions. Since $A$ has [full row rank](full-row-rank.md), its [Moore-Penrose inverse](moore-penrose-inverse.md) is

$$
A^+=A^T(AA^T)^{-1}
=\frac15\begin{pmatrix}1\\2\end{pmatrix},
\qquad
\boxed{x_*=A^+b=(3/5,6/5)^T.}
$$

The [kernel](kernel-of-a-linear-map-split.md) is $\operatorname{span}\{(-2,1)^T\}$, and all exact solutions are

$$
x=x_*+t(-2,1)^T,\qquad t\in\mathbb R.
$$

Because $x_*$ is [orthogonal](orthogonal-vectors.md) to $(-2,1)^T$,

$$
\|x\|_2^2=\frac95+5t^2.
$$

The [Euclidean norm](euclidean-norm.md) is therefore smallest exactly at $t=0$. The zero residual alone cannot select a solution; the minimum-norm rule supplies the additional criterion.

<a id="image-the-minimum-norm-solution-is-the-closest-point-of-the-solution-line-to-the-origin"></a>
![](pseudoinverse-minimum-norm-line.png)

**[Figure 5](#image-the-minimum-norm-solution-is-the-closest-point-of-the-solution-line-to-the-origin). The minimum-norm solution is the closest point of the solution line to the origin**. The [affine line](affine-line.md) $x_1+2x_2=3$ is perpendicular to $x_*=(3/5,6/5)^T$. Moving along the line changes only a [kernel](kernel-of-a-linear-map-split.md) component and increases $\|x\|_2^2$ by $5t^2$.

This selection depends on the specified [inner product](inner-product-split.md). Rescaling one unknown changes what counts as a small [Euclidean norm](euclidean-norm.md), so units and weighting matter in an application. A minimum-norm answer is mathematically canonical for the chosen geometry, rather than an automatic guarantee of physical plausibility.

## ↑ Ancestors (7)

1. [Moore-Penrose inverse](moore-penrose-inverse.md)
2. [Matrix inverse](matrix-inverse-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
