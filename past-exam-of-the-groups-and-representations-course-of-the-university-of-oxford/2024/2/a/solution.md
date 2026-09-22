<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the mathematical [Lie algebra](../../../../lie-algebra-split.md) convention $U(t)=I+tX+O(t^2)$. Differentiating $U^\dagger U=I$ and $\det U=1$ at $t=0$ gives $X^\dagger=-X$ and $\operatorname{tr}X=0$. Conversely, for such an $X$, the [matrix exponential](../../../../matrix-exponential.md) is unitary and has [determinant](../../../../determinant.md) $\det e^{tX}=e^{t\operatorname{tr}X}=1$. Thus

$$
\boxed{\mathfrak{su}(4)=\{X\in M_4(\mathbb C):X^\dagger=-X,\ \operatorname{tr}X=0\},
\qquad [X,Y]=XY-YX.}
$$

The four diagonal entries are purely imaginary, and the six entries above the diagonal are arbitrary [complex numbers](../../../../complex-number.md) determining the entries below it. This gives $4+2\cdot6=16$ real parameters before imposing the one real [trace](../../../../matrix-trace.md) constraint, so $\dim_{\mathbb R}\mathfrak{su}(4)=15$.

A [Cartan subalgebra](../../../../cartan-subalgebra.md) of this compact [Lie algebra](../../../../lie-algebra-split.md) is a maximal commuting [Lie subalgebra](../../../../lie-subalgebra.md); choose

$$
\mathfrak h=\{i\operatorname{diag}(h_1,h_2,h_3,h_4):h_i\in\mathbb R,\ \sum_i h_i=0\}.
$$

A simple [basis](../../../../basis.md) is $iH_1,iH_2,iH_3$, where

$$
H_1=\operatorname{diag}(1,-1,0,0),\quad
H_2=\operatorname{diag}(0,1,-1,0),\quad
H_3=\operatorname{diag}(0,0,1,-1).
$$

Any [matrix](../../../../matrix.md) commuting with every diagonal element is itself diagonal, which proves maximality. Commuting [skew-Hermitian matrices](../../../../skew-hermitian-matrix.md) can also be simultaneously diagonalized, so no larger commuting [Lie subalgebra](../../../../lie-subalgebra.md) is possible. Consequently

$$
\boxed{\dim\mathfrak{su}(4)=15,\qquad\operatorname{rank}\mathfrak{su}(4)=\dim\mathfrak h=3.}
$$

The [Hermitian quantum generator convention](../../../../hermitian-quantum-generator-convention.md) instead uses the Hermitian $H_a$ and $U=\exp(i\theta^aH_a)$. The two conventions describe the same [Lie algebra](../../../../lie-algebra-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
