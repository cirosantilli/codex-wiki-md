<h1 id="39c/solution">Solution</h1>

↑ **Parent:** [39C](../39c.md)

Work in the [shock frame](../../../../../shock-frame.md). The undisturbed upstream gas enters the stationary discontinuity at speed

$$
w_1=U,
$$

while the downstream gas, which moves with the piston in the laboratory frame, leaves at

$$
w_2=U-V.
$$

The [Rankine-Hugoniot conditions for a perfect gas](../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md) are

$$
\rho_1U=\rho_2(U-V),
$$



$$
p_1+\rho_1U^2
=p_2+\rho_2(U-V)^2,
$$

and

$$
\frac{\gamma p_1}{(\gamma-1)\rho_1}+\frac{U^2}{2}
=\frac{\gamma p_2}{(\gamma-1)\rho_2}
+\frac{(U-V)^2}{2}.
$$

Eliminating the velocities between these equations gives the perfect-gas density jump

$$
\frac{\rho_2}{\rho_1}
=\frac{2\gamma+(\gamma+1)\beta}
{2\gamma+(\gamma-1)\beta},
\qquad
p_2=(1+\beta)p_1.
$$

The mass and momentum equations also imply

$$
p_2-p_1
=\rho_1U^2-\rho_2(U-V)^2
=\rho_1UV,
$$

so

$$
V=\frac{\beta p_1}{\rho_1U}.
$$

Substitution of the density ratio into mass conservation, followed by this momentum relation, gives

$$
U^2=\frac{p_1}{\rho_1}
\left[\gamma+\frac{\gamma+1}{2}\beta\right].
$$

Using the [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) $c_1^2=\gamma p_1/\rho_1$ therefore yields

$$
\boxed{\frac{U^2}{c_1^2}
=1+\frac{\gamma+1}{2\gamma}\beta.}
$$

Finally, eliminating $U$ from $V=\beta p_1/(\rho_1U)$ gives the [piston-driven normal shock](../../../../../piston-driven-normal-shock.md) relation

$$
\boxed{
V^2=
\frac{2\beta^2}{2\gamma+(\gamma+1)\beta}
\frac{p_1}{\rho_1}.}
$$

For a compressive shock $\beta>0$, the first boxed equation has $U>c_1$: **the shock propagates supersonically into the undisturbed gas**, approaching the sound speed in the [weak shock](../../../../../weak-shock.md) limit $\beta\to0$.

## ↑ Ancestors (10)

1. [39C](../39c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
