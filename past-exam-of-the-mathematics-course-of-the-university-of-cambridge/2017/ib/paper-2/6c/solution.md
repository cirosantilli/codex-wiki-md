<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

In electrostatics, [Gauss's law](../../../../../gauss-s-law.md) is $\oint_{\partial\Omega}\mathbf E\cdot\mathbf n\,dS=Q_{\rm enclosed}/\epsilon_0$, or locally $\nabla\cdot\mathbf E=\rho_e/\epsilon_0$, where $\rho_e$ is charge density and $\epsilon_0$ is [vacuum permittivity](../../../../../vacuum-permittivity.md). [Spherical symmetry](../../../../../spherical-symmetry.md) makes the [electric field](../../../../../electric-field.md) radial, and Gauss's law gives

$$
\boxed{\mathbf E(r)=\begin{cases}0,&r<a,\\ \dfrac{Q}{4\pi\epsilon_0r^2}\mathbf e_r,&a<r<b,\\0,&r>b.\end{cases}}
$$

Choose the additive constant of the [electrostatic potential](../../../../../electric-potential.md) by $\phi(\infty)=0$. Using $\mathbf E=-\nabla\phi$ and continuity of potential across each charged shell gives

$$
\boxed{\phi(r)=\begin{cases}\dfrac{Q}{4\pi\epsilon_0}(1/a-1/b),&r<a,\\ \dfrac{Q}{4\pi\epsilon_0}(1/r-1/b),&a<r<b,\\0,&r>b.\end{cases}}
$$

The field jumps at the shell surfaces, so the displayed formulas are for the requested open regions. The potential difference of the [spherical capacitor](../../../../../spherical-capacitor.md) is $\Delta\phi=Q(1/a-1/b)/(4\pi\epsilon_0)$. Thus its [capacitance](../../../../../capacitance.md) and [electrostatic energy](../../../../../electrostatic-energy.md) are

$$
\boxed{C=\frac{Q}{\Delta\phi}=\frac{4\pi\epsilon_0ab}{b-a},\qquad W=\frac{Q^2}{2C}.}
$$

The energy follows either by charging work $\int_0^Q q/C\,dq$, or directly from $W=(\epsilon_0/2)\int|\mathbf E|^2\,d^3x=Q^2(1/a-1/b)/(8\pi\epsilon_0)$.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
