<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Differentiate the defining relation at $\Lambda=I+tX+O(t^2)$. The linear term gives the [Lie algebra](../../../../lie-algebra-split.md)

$$
\mathfrak g=\{X\in M_3(\mathbb R):X^T\eta+\eta X=0\}.
$$

Solving this equation between [matrices](../../../../matrix.md) yields

$$
X=\begin{pmatrix}0&a&b\\a&0&-c\\b&c&0\end{pmatrix}
=aK_1+bK_2+cJ,
$$

where a convenient [basis](../../../../basis.md) is

$$
K_1=\begin{pmatrix}0&1&0\\1&0&0\\0&0&0\end{pmatrix},\qquad
K_2=\begin{pmatrix}0&0&1\\0&0&0\\1&0&0\end{pmatrix},\qquad
J=\begin{pmatrix}0&0&0\\0&0&-1\\0&1&0\end{pmatrix}.
$$

The first two generate [Lorentz boosts](../../../../lorentz-boost.md) and the last a spatial [rotation](../../../../rotation-mathematics.md). Direct [commutators](../../../../commutator.md) give

$$
\boxed{[J,K_1]=K_2,\qquad[J,K_2]=-K_1,\qquad[K_1,K_2]=-J.}
$$

There are three independent real coefficients, so $\dim_{\mathbb R}\mathfrak g=3$. A [Cartan subalgebra](../../../../cartan-subalgebra.md) is $\mathbb RJ$, and the [rank of a semisimple Lie algebra](../../../../rank-of-a-semisimple-lie-algebra.md) is one. Explicitly, if $X=aK_1+bK_2+cJ$ and $Y=a'K_1+b'K_2+c'J$, their [commutator](../../../../commutator.md) vanishes exactly when

$$
bc'-cb'=ca'-ac'=ba'-ab'=0.
$$

For nonzero $X$, these equations force $Y$ to be proportional to $X$, so there is no two-dimensional commuting [subalgebra](../../../../subalgebra.md). The split real rank is also one, realized by the semisimple [Lorentz boost](../../../../lorentz-boost.md) generator $K_1$. Thus

$$
\boxed{\mathfrak g=\mathfrak{so}(1,2),\qquad\dim\mathfrak g=3,\qquad\operatorname{rank}\mathfrak g=1.}
$$

For this [Lorentz algebra in three spacetime dimensions](../../../../lorentz-algebra-in-three-spacetime-dimensions.md), disconnected components of the full [Lorentz group](../../../../lorentz-group.md) do not change its tangent [Lie algebra](../../../../lie-algebra-split.md) at the identity.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
