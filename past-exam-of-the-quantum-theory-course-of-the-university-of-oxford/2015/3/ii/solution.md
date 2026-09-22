<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the [Frobenius method](../../../../frobenius-method.md) at the origin. The lowest power in $f''-\ell(\ell+1)f/r^2$ is $r^{c-2}$, with coefficient

$$
\bigl[c(c-1)-\ell(\ell+1)\bigr]a_0.
$$

The terms $-2\alpha f'$ and $2mKZf/(\hbar^2r)$ start at power $r^{c-1}$ and therefore cannot cancel a nonzero $r^{c-2}$ coefficient. Because $a_0\ne0$, the [indicial equation](../../../../indicial-equation.md) is

$$
\boxed{c(c-1)-\ell(\ell+1)=0,\qquad (c-\ell-1)(c+\ell)=0.}
$$

Its roots are $c=\ell+1$ and $c=-\ell$. Since $\psi=r^{-1}f e^{-\alpha r}$, their leading behaviors are respectively $\psi\sim r^\ell$ and $\psi\sim r^{-\ell-1}$. The physical choice is

$$
\boxed{c=\ell+1.}
$$

This is the [Coulomb radial origin condition](../../../../coulomb-radial-origin-condition.md). For $\ell\geq1$, the other branch is not even locally normalizable: its radial [probability](../../../../probability.md) integral behaves as $\int_0^\varepsilon r^2r^{-2\ell-2}\,dr=\int_0^\varepsilon r^{-2\ell}\,dr$, which diverges.

For $\ell=0$, the singular behavior $1/r$ is locally [square-integrable](../../../../square-integrable-function.md) with the measure $r^2dr$, so local [wavefunction normalization](../../../../wavefunction-normalization.md) alone would not reject it. The ordinary three-dimensional [Coulomb potential](../../../../coulomb-potential-energy.md) problem additionally requires the regular [boundary condition](../../../../boundary-condition.md) $u(0)=0$. A $1/r$ branch violates that condition and has divergent [kinetic energy](../../../../kinetic-energy.md) integral $\int_0^\varepsilon r^2|\partial_r(1/r)|^2\,dr=\int_0^\varepsilon r^{-2}\,dr$. Thus it is excluded from the physical energy domain as well. The regular choice gives $u\sim r^{\ell+1}$ in every case.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
