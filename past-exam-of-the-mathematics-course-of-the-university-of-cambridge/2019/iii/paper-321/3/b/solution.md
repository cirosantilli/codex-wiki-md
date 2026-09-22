<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $H=z^+$ and $B_+=B_x^+$, and assume $B_z\ne0$ and $q>0$. In a [steady state](../../../../../../steady-state.md), the [horizontally invariant magnetized shearing-sheet equations](../../../../../../horizontally-invariant-magnetized-shearing-sheet-equations.md) give

$$
v_x'=0,\qquad
B_y'=\frac{\mu_0\rho}{B_z}(2-q)\Omega v_x.
$$

Since $B_y$ vanishes at both boundaries, $v_x=0$ for $q\ne2$, and then $B_y=0$ throughout. The other two equations are

$$
v_y=-\frac{B_z}{2\mu_0\rho\Omega}B_x',\qquad
v_y'=\frac{q\Omega}{B_z}B_x.
$$

Eliminating $v_y$ gives the [harmonic oscillator equation](../../../../../../simple-harmonic-motion.md)

$$
B_x''+K^2B_x=0,\qquad
K^2=\frac{2q\mu_0\rho\Omega^2}{B_z^2}.
$$

The midplane-symmetric [magnetic bending in an incompressible disk](../../../../../../magnetic-bending-in-an-incompressible-disk.md) has odd $B_x$ and even $v_y$. Applying $B_x(\pm H)=\pm B_+$ gives

$$
\boxed{B_x=B_+\frac{\sin(Kz)}{\sin(KH)},\qquad B_y=0,\qquad v_x=0},
$$



$$
\boxed{v_y=-\frac{B_zKB_+}{2\mu_0\rho\Omega\sin(KH)}\cos(Kz)}.
$$

For nonzero imposed inclination $B_+$, this equilibrium exists only when $\sin(KH)\ne0$. More generally, $B_x=A\sin(Kz)+D\cos(Kz)$; the [boundary conditions](../../../../../../boundary-condition.md) require $A\sin(KH)=B_+$ and $D\cos(KH)=0$. Thus the displayed solution is unique away from these resonances. At $\cos(KH)=0$, an additional even homogeneous solution is possible unless midplane symmetry is imposed. At $q=2$, an arbitrary constant $v_x$ is also allowed because its coefficient in the azimuthal equation vanishes; choosing $v_x=0$ gives the same symmetric equilibrium.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
