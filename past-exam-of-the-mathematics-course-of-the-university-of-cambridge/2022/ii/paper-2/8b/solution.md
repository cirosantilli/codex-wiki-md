<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Order the phase-space coordinates as

$$
x=(q_1,\ldots,q_n,p_1,\ldots,p_n),
\qquad
\Omega=\begin{pmatrix}0&I\\-I&0\end{pmatrix}.
$$

Then [Hamilton's equations](../../../../../hamilton-s-equations.md) are

$$
\dot x_a=\Omega_{ab}\frac{\partial H}{\partial x_b}.
$$

The [Poisson bracket](../../../../../poisson-bracket.md) is

$$
\{f,g\}=\frac{\partial f}{\partial x_a}
\Omega_{ab}\frac{\partial g}{\partial x_b},
\qquad
\boxed{\{x_a,x_b\}=\Omega_{ab}}.
$$

For $X=X(x)$ with Jacobian $J_{ab}=\partial X_a/\partial x_b$, the chain rule gives

$$
\dot X=J\Omega J^T\nabla_XH.
$$

This has Hamiltonian form with the same canonical matrix for every $H$ exactly when

$$
\boxed{J\Omega J^T=\Omega}.
$$

Taking determinants gives $(\det J)^2=1$; the symplectic condition fixes the orientation, so $\det J=1$. Hence the change-of-variables formula shows that the phase-space volume element is invariant. This is [Liouville theorem in Hamiltonian mechanics](../../../../../liouville-s-theorem-hamiltonian.md).

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
