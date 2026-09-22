<h1 id="j/j1/solution">Solution</h1>

↑ **Parent:** [J1](../j1.md)

For a real potential, the time-dependent [Schrödinger equation](../../../../schrodinger-equation.md) is

$$
\boxed{i\hbar\partial_t\psi=-\frac{\hbar^2}{2m}\Delta\psi+V\psi.}
$$

Multiply it by $\psi^*$, combine with its conjugate multiplied by $\psi$, and note that the real-potential terms cancel. This gives

$$
\partial_t|\psi|^2=\frac{i\hbar}{2m}(\psi^*\Delta\psi-\psi\Delta\psi^*)
=-\nabla\cdot\mathbf j,
$$

where the [probability current](../../../../probability-current.md) is

$$
\boxed{\mathbf j=\frac{\hbar}{2mi}(\psi^*\nabla\psi-\psi\nabla\psi^*)
=\frac\hbar m\operatorname{Im}(\psi^*\nabla\psi).}
$$

The product rule gives the divergence identity because the gradient cross terms cancel.

For $F(r)=\sin(kr)/r$, the supplied radial identity gives $\Delta F=-k^2F$ for $r>0$. The time factor gives $i\hbar\psi_t=E\psi$, so the free equation holds for

$$
\boxed{k=\frac{\sqrt{2mE}}\hbar.}
$$

The apparent origin singularity is removable: $F(0)=k$ and $F(r)=k-k^3r^2/6+\cdots$, so the equation extends smoothly there as well. Since the spatial factor is real and its time dependence is a common phase, $\psi^*\nabla\psi=F\nabla F$ is real. Thus $\mathbf j=0$, while $\rho=F^2$ is independent of time. Both terms in the [continuity equation](../../../../continuity-equation.md) vanish separately. This is a standing [spherical wave](../../../../spherical-wave.md); the real spatial factor carries no net radial [probability current](../../../../probability-current.md).

## ↑ Ancestors (12)

1. [J1](../j1.md)
2. [J](../../j.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
