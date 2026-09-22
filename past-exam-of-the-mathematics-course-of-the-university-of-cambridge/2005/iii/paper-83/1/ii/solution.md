<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the uniform background [number density](../../../../../../number-density.md) be $n_\infty>0$ and set $\mu=Un_\infty$. The subtraction of this [chemical potential](../../../../../../chemical-potential.md) requires a phase rotation as well as a rescaling:

$$
\psi_{\rm phys}(\mathbf x,t)=\sqrt{n_\infty}\,e^{-i\mu t/\hbar}\Psi(\widetilde{\mathbf x},\widetilde t),
\qquad \widetilde{\mathbf x}=\frac{\mathbf x}{\ell_0},\quad \widetilde t=\frac t{t_0}.
$$

Substitution into the physical [Gross–Pitaevskii equation](../../../../../../gross-pitaevskii-equation.md) gives

$$
i\frac{\hbar}{\mu t_0}\Psi_{\widetilde t}
=-\frac{\hbar^2}{2m\mu\ell_0^2}\widetilde\nabla^2\Psi+(|\Psi|^2-1)\Psi.
$$

Consequently the requested coefficients follow from

$$
\boxed{\ell_0=\frac{\hbar}{\sqrt{2m\mu}},\qquad t_0=\frac{\hbar}{2\mu},\qquad \psi\text{ unit}=\sqrt{\mu/U}.}
$$

The length unit is the specified [healing length](../../../../../../healing-length.md). Removing tildes produces the paper's dimensionless equation; in particular the coefficient of its time derivative fixes $t_0$, not its reciprocal. Without the phase rotation the linear $+\Psi$ term would not appear.

The dimensionless [ground state](../../../../../../ground-state.md) is **$\Psi=e^{i\chi}$ for any constant phase $\chi$**, conventionally $\Psi=1$. Its subtracted energy is proportional to $\int[|\nabla\Psi|^2+(1-|\Psi|^2)^2/2]d^3x$, which is nonnegative and vanishes for this state. In physical variables it has density $n_\infty$ and phase rotating at $\mu/\hbar$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
