<h1 id="36b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [magnetization](../../../../../../magnetization.md) $\mathbf M$ is magnetic dipole moment per unit volume. In magnetostatics it produces

$$
\mathbf J_{\rm b}=\nabla\times\mathbf M,
\qquad
\mathbf K_{\rm b}=\mathbf M\times\mathbf n.
$$

The [magnetic field intensity](../../../../../../magnetic-field-intensity.md) $\mathbf H=\mathbf B/\mu_0-\mathbf M$ obeys

$$
\nabla\times\mathbf H=\mathbf J_{\rm free},
$$

so $\mathbf H$ isolates free currents while $\mathbf M$ accounts for bound currents. For a linear isotropic material, $\mathbf B=\mu\mathbf H$.

Ampere's law for a circular loop around the free line current gives

$$
\mathbf H=\frac{I}{2\pi r}\mathbf e_\phi
$$

in both media. Therefore

$$
\mathbf M_i
=\left(\frac{\mu_i}{\mu_0}-1\right)
\frac{I}{2\pi r}\mathbf e_\phi.
$$

At $r=R$, the net bound surface-current density is

$$
\begin{aligned}
\mathbf K_{\rm b}
&=(\mathbf M_1-\mathbf M_2)\times\mathbf e_r\\
&=-\frac{I(\mu_1-\mu_2)}
{2\pi R\mu_0}\mathbf e_z.
\end{aligned}
$$

Hence its magnitude is

$$
\boxed{|\mathbf K_{\rm b}|=
\frac{I|\mu_1-\mu_2|}{2\pi R\mu_0}},
$$

and for a positive current along $+\mathbf e_z$ it points along $-\mathbf e_z$ when $\mu_1>\mu_2$, reversing when $\mu_1<\mu_2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [36B](../../36b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
