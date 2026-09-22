<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $A=\mathbf p\cdot\boldsymbol\sigma$ and $E=\sqrt{\mathbf p^2+m^2}$. The [Pauli multiplication identity](../../../../pauli-multiplication-identity.md) gives $A^2=\mathbf p^2I_2$, and the orthonormal two-component [spinors](../../../../spinor.md) obey $\sum_s\xi^s\xi^{s\dagger}=I_2$. Taking the [Dirac adjoint](../../../../dirac-adjoint.md) of the supplied [Dirac spinor](../../../../dirac-spinor.md) therefore gives, directly,

$$
\begin{aligned}
\sum_su^s(\mathbf p)\bar u^s(\mathbf p)
&=\begin{pmatrix}(E+m)I_2&-A\\ A&-A^2/(E+m)\end{pmatrix}\\
&=\begin{pmatrix}(E+m)I_2&-A\\ A&(m-E)I_2\end{pmatrix}
=\boxed{\not p+m}.
\end{aligned}
$$

For the antiparticle deduction, specify the standard normalization $v^{r\dagger}(-\mathbf p)v^s(-\mathbf p)=2E\delta^{rs}$, just as $u^{r\dagger}u^s=2E\delta^{rs}$. **Spanning alone does not specify a normalization:** replacing every $v$ by $2v$ preserves the spanning property but multiplies its proposed [fermion spin sum](../../../../fermion-spin-sum.md) by four. The standard normalization is the convention implicit in the [mode expansion of a Dirac field](../../../../mode-expansion-of-a-dirac-field.md) with the standard [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md).

To use completeness correctly, introduce the [Hermitian](../../../../hermitian-operator.md) [Dirac Hamiltonian](../../../../dirac-hamiltonian.md)

$$
h(\mathbf p)=\boldsymbol\alpha\cdot\mathbf p+\beta m,
\qquad\alpha^i=\gamma^0\gamma^i,\quad\beta=\gamma^0.
$$

The [Dirac equation](../../../../dirac-equation.md) makes $u^s(\mathbf p)$ and $v^s(-\mathbf p)$ its [eigenvectors](../../../../eigenvector.md) with [eigenvalues](../../../../eigenvalue.md) $E$ and $-E$. Their mutual orthogonality and spanning property give complementary [orthogonal projectors](../../../../orthogonal-projection.md)

$$
\frac1{2E}\sum_su^s(\mathbf p)u^{s\dagger}(\mathbf p)=\frac{E+h(\mathbf p)}{2E},\qquad
\frac1{2E}\sum_sv^s(-\mathbf p)v^{s\dagger}(-\mathbf p)=\frac{E-h(\mathbf p)}{2E}.
$$

Multiply the second equality by $2E\gamma^0$ on the right and replace $\mathbf p$ by $-\mathbf p$. For the positive-energy [four-momentum](../../../../four-momentum.md) $p=(E,\mathbf p)$,

$$
[E-h(-\mathbf p)]\gamma^0
=E\gamma^0-\boldsymbol\gamma\cdot\mathbf p-m=\not p-m,
\qquad\boxed{\sum_sv^s(\mathbf p)\bar v^s(\mathbf p)=\not p-m}.
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
