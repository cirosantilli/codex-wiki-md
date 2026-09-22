<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For unit mass, the [Lagrangian](../../../../../../lagrangian.md) in [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) is

$$
L=\frac12\left(\dot r^2+r^2\dot\varphi^2+\dot z^2\right)-\Phi(r,z).
$$

Introduce [shearing sheet](../../../../../../shearing-sheet.md) coordinates by $r=r_0+x$ and $\varphi=\Omega_0t+y/r_0$. Evaluate all derivatives of $\Phi$ at $(r_0,0)$. The reference [circular orbit](../../../../../../circular-orbit.md) obeys $\Phi_r=r_0\Omega_0^2$, while midplane symmetry gives $\Phi_z=\Phi_{rz}=0$. Its [Taylor expansion](../../../../../../taylor-expansion.md) is

$$
\Phi=\Phi_0+\Phi_rx+\frac12\Phi_{rr}x^2+\frac12\Phi_{zz}z^2+O(3).
$$

Expanding the kinetic energy to the same order gives

$$
\frac12r^2\dot\varphi^2
=\frac12r_0^2\Omega_0^2+r_0\Omega_0^2x+r_0\Omega_0\dot y
+\frac12\Omega_0^2x^2+2\Omega_0x\dot y+\frac12\dot y^2+O(3).
$$

The terms linear in $x$ cancel by circular-orbit balance. Discard the constant and the term $r_0\Omega_0\dot y$ by [total-time-derivative invariance of a Lagrangian](../../../../../../total-time-derivative-invariance-of-a-lagrangian.md); these do not change the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md). The [particle Lagrangian in a shearing sheet](../../../../../../particle-lagrangian-in-a-shearing-sheet.md) is therefore

$$
\boxed{L_2=\frac12(\dot x^2+\dot y^2+\dot z^2)+2\Omega_0x\dot y-\Phi_t},
$$

with [shearing-sheet tidal potential](../../../../../../shearing-sheet-tidal-potential.md)

$$
\boxed{\Phi_t=\frac12(\Phi_{rr}-\Omega_0^2)x^2+\frac12\Phi_{zz}z^2
=-q_0\Omega_0^2x^2+\frac12\Omega_z^2z^2}.
$$

The second form follows from $\Phi_r=r\Omega^2$, the [orbital shear parameter](../../../../../../orbital-shear-parameter.md) $q_0=-d\log\Omega/d\log r$ and the [vertical epicyclic frequency](../../../../../../vertical-epicyclic-frequency.md) $\Omega_z^2=\Phi_{zz}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
