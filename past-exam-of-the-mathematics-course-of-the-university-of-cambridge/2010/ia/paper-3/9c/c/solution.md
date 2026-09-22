<h1 id="9c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $i\ne j$, the inertia component is $I_{ij}=-\rho\int_V x_ix_j\,dV$. Reflecting just one of these coordinates preserves the cylinder and its uniform density but changes the integrand's sign. [Odd-integrand cancellation by reflection](../../../../../../odd-integrand-cancellation-by-reflection.md) therefore makes every off-diagonal entry zero. Rotations about the axis also give $I_{11}=I_{22}$.

Using [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) $x_1=r\cos\theta$, $x_2=r\sin\theta$, $x_3=z$, with $dV=r\,dr\,d\theta\,dz$, the required integrals are

$$
\begin{aligned}
\int_Vx_2^2\,dV&=4\left(\int_0^1r^3\,dr\right)\left(\int_0^{2\pi}\sin^2\theta\,d\theta\right)=\pi,\\
\int_Vz^2\,dV&=\left(\int_{-2}^{2}z^2\,dz\right)\left(\int_0^1r\,dr\right)\left(\int_0^{2\pi}d\theta\right)=\frac{16\pi}{3},\\
\int_V(x_1^2+x_2^2)\,dV&=4\left(\int_0^1r^3\,dr\right)2\pi=2\pi.
\end{aligned}
$$

Thus the [inertia tensor](../../../../../../inertia-tensor.md) is

$$
\boxed{I=\rho\pi\operatorname{diag}\left(\frac{19}{3},\frac{19}{3},2\right).}
$$

The mass is $M=4\pi\rho$, so these entries are also $19M/12,19M/12,M/2$, respectively.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9C](../../9c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
