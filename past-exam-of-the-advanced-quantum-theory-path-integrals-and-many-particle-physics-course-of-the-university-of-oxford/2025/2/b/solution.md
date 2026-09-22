<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Writing the [Bogoliubov transformation](../../../../bogoliubov-transformation.md) componentwise, together with its [Hermitian adjoint](../../../../adjoint-operator.md), gives

$$
a=uc+vd^\dagger,\qquad b=-vc^\dagger+ud,\qquad
a^\dagger=uc^\dagger+vd,\qquad b^\dagger=-vc+ud^\dagger.
$$

The full [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) for $c,d$ imply

$$
\{a,a^\dagger\}=u^2\{c,c^\dagger\}+v^2\{d^\dagger,d\}=u^2+v^2,
\qquad \{b,b^\dagger\}=u^2+v^2.
$$

Equal-type [anticommutators](../../../../anticommutator.md) vanish because $c^2=d^2=0$ and $\{c,d^\dagger\}=\{c^\dagger,d\}=0$:

$$
\{a,a\}=\{b,b\}=0.
$$

For the mixed [anticommutators](../../../../anticommutator.md), the only potentially nonzero terms cancel:

$$
\{a,b\}=-uv\{c,c^\dagger\}+uv\{d^\dagger,d\}
=-uv+uv=0,
$$

while $\{a,b^\dagger\}=0$ follows from $\{c,c\}=\{d^\dagger,d^\dagger\}=\{c,d^\dagger\}=0$. Taking the [Hermitian adjoint](../../../../adjoint-operator.md) supplies the remaining relations. Thus the necessary and sufficient condition is

$$
\boxed{u^2+v^2=1.}
$$

Equivalently, the [matrix](../../../../matrix.md) $R=\begin{pmatrix}u&v\\-v&u\end{pmatrix}$ is an [orthogonal matrix](../../../../orthogonal-matrix.md), $R^{\mathsf T}R=I$, giving a [canonical rotation of two fermionic modes](../../../../canonical-rotation-of-two-fermionic-modes.md). Its inverse is therefore

$$
\boxed{c=ua-vb^\dagger,\qquad d=va^\dagger+ub.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
