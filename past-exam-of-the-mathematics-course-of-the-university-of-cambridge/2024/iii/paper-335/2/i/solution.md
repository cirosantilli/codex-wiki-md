<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the sign convention in the question,

$$
V(\mathbf r)=k_0^2[n^2(\mathbf r)-1].
$$

Then the total field satisfies

$$
(\nabla^2+k_0^2)\psi=-V\psi.
$$

The outgoing free-space [Green function](../../../../../../green-s-function.md) is

$$
G_0(\mathbf r-\mathbf r')
=\frac{e^{ik_0|\mathbf r-\mathbf r'|}}
{4\pi|\mathbf r-\mathbf r'|},
$$

with $(\nabla^2+k_0^2)G_0=-\delta$. Hence the [Lippmann-Schwinger equation](../../../../../../lippmann-schwinger-equation.md) is

$$
\psi(\mathbf r)=\psi_i(\mathbf r)
+\int_DG_0(\mathbf r-\mathbf r')
V(\mathbf r')\psi(\mathbf r')\,d^3r'.
$$

Replacing the unknown interior total field by the incident field gives the first [Born approximation](../../../../../../born-approximation.md)

$$
\boxed{
\psi_B(\mathbf r)=\psi_i(\mathbf r)
+\int_DG_0(\mathbf r-\mathbf r')
V(\mathbf r')\psi_i(\mathbf r')\,d^3r'}.
$$

For the [Rytov approximation](../../../../../../rytov-approximation.md), put $\psi=\psi_i e^\phi$. After division by $\psi$, the wave equation gives

$$
\nabla^2\phi+(\nabla\phi)^2
+2\nabla\log\psi_i\mathbin\cdot\nabla\phi
=-V.
$$

Neglecting the quadratic term $(\nabla\phi)^2$ makes $\psi_i\phi$ obey the same inhomogeneous equation as the first Born scattered field. Thus

$$
\phi_1(\mathbf r)
=\frac1{\psi_i(\mathbf r)}
\int_DG_0(\mathbf r-\mathbf r')
V(\mathbf r')\psi_i(\mathbf r')\,d^3r',
$$

and

$$
\boxed{
\psi_R(\mathbf r)=\psi_i(\mathbf r)e^{\phi_1(\mathbf r)}}.
$$

Its [power series](../../../../../../power-series.md) begins

$$
\psi_R=\psi_i(1+\phi_1+O(\phi_1^2))
=\psi_B+O(V^2),
$$

so the two approximations agree through first order in the [scattering potential](../../../../../../scattering-potential.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
