<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $I=RB_\phi$ and define $\Delta_*\psi=\psi_{RR}-R^{-1}\psi_R+\psi_{zz}$. Direct cylindrical differentiation gives

$$
(\nabla\times B)_R=-I_z/R,\quad
(\nabla\times B)_z=I_R/R,\quad
(\nabla\times B)_\phi=-\Delta_*\psi/R.
$$

The azimuthal component of the [Lorentz force](../../../../../../lorentz-force.md) is proportional to $I_z\psi_R-I_R\psi_z$. A [force-free magnetic field](../../../../../../force-free-magnetic-field.md) therefore has parallel meridional gradients of $I$ and $\psi$, implying $I=f(\psi)$ on connected regular flux surfaces. Consequently

$$
\boxed{B_\phi=f(\psi)/R.}
$$

With this dependence the poloidal part of $\nabla\times B$ is $f'(\psi)B_p$. Its full cross product with $B$ is

$$
(\nabla\times B)\times B
=-\frac{\Delta_*\psi+f(\psi)f'(\psi)}{R^2}\nabla\psi.
$$

Vanishing force therefore requires $\Delta_*\psi+ff'=0$ wherever the flux gradient is nonzero, extending by regularity through ordinary isolated nulls. Finally, evaluating the three-dimensional cylindrical divergence gives $R^2\nabla\cdot(R^{-2}\nabla\psi)=\Delta_*\psi$, so

$$
\boxed{R^2\nabla\cdot(R^{-2}\nabla\psi)+f\frac{df}{d\psi}=0.}
$$

This derives the [Grad-Shafranov equation for a force-free magnetic field](../../../../../../grad-shafranov-equation-for-a-force-free-magnetic-field.md). The function $f$ is set by boundary/current information; it is not an additional fixed constant. Its single-valued global form presumes the usual connected flux-surface labeling. The equation also makes $\nabla\times B=f'(\psi)B$, explicitly showing that current is parallel to the [magnetic field](../../../../../../magnetic-field.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
