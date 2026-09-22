<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Adding the two homogeneous reaction rates gives $a-u$, so the unique positive [Brusselator](../../../../../../brusselator.md) equilibrium is

$$
\boxed{u_*=a,\qquad v_*=b/a.}
$$

The reaction [Jacobian matrix](../../../../../../jacobian-matrix.md) at that state is

$$
J=\begin{pmatrix}b-1&a^2\\-b&-a^2\end{pmatrix},\qquad
\tau=\operatorname{tr}J=b-1-a^2,\qquad\Delta=\det J=a^2.
$$

A real two-dimensional linear system has strict [asymptotic stability](../../../../../../asymptotic-stability.md) exactly when $\tau<0$ and $\Delta>0$: the [eigenvalues](../../../../../../eigenvalue.md) solve $\lambda^2-\tau\lambda+\Delta=0$. Real [eigenvalues](../../../../../../eigenvalue.md) then have positive product and negative sum; a complex conjugate pair has real part $\tau/2$. Conversely, stable [eigenvalues](../../../../../../eigenvalue.md) require those signs.

Since $a>0$, the [Brusselator](../../../../../../brusselator.md) is homogeneously stable precisely for

$$
\boxed{b<1+a^2.}
$$

At $b_H=1+a^2$, the linear [eigenvalues](../../../../../../eigenvalue.md) are $\pm ia$, so strict decay is lost through a homogeneous [Hopf bifurcation](../../../../../../hopf-bifurcation.md) threshold. For larger $b$ the equilibrium is unstable. The source's matrix label $A$ is here written $J$ to distinguish it from the filament modulus in the preceding question.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
