<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Seek $\psi=\Psi(x)\cos(my)$, with $m=\pi/b$. The [ordinary differential equation](../../../../ordinary-differential-equation.md) is

$$
r\Psi''+\beta\Psi'-rm^2\Psi=F_0.
$$

Its constant particular solution and characteristic exponents are

$$
\boxed{A=-\frac{F_0}{rm^2}=-\frac{F_0b^2}{r\pi^2},\qquad
\lambda=\frac{\beta+\sqrt{\beta^2+4r^2m^2}}{2r},\qquad
\gamma=\frac{\sqrt{\beta^2+4r^2m^2}-\beta}{2r}.}
$$

Both $\lambda,\gamma$ are positive; the two homogeneous solutions are $e^{-\lambda x}$ and $e^{\gamma x}$. Their product satisfies $\lambda\gamma=m^2$. At small $rm/\beta$,

$$
\boxed{\lambda\simeq\frac\beta r,\qquad \gamma\simeq\frac{rm^2}\beta.}
$$

For the rectangular basin, choose zero [streamfunction](../../../../stream-function.md) on its connected impermeable boundary. The factor $\cos(my)$ already gives zero at $y=\pm b/2$. Enforcing $\Psi(0)=\Psi(L)=0$ yields the exact result

$$
\Psi=A\left[1-C_W e^{-\lambda x}-C_E e^{\gamma(x-L)}\right],
$$

where

$$
C_W=\frac{1-e^{-\gamma L}}{1-e^{-(\lambda+\gamma)L}},\qquad
C_E=\frac{1-e^{-\lambda L}}{1-e^{-(\lambda+\gamma)L}}.
$$

The narrow [Stommel boundary layer](../../../../stommel-boundary-layer.md) approximation requires

$$
\boxed{\lambda^{-1}\ll L\ll\gamma^{-1}.}
$$

Then $e^{-\lambda L}$ is negligible, $C_W\simeq\gamma L$ and $C_E\simeq1$, giving

$$
\boxed{\psi\simeq A\left[1-\gamma L e^{-\lambda x}-e^{\gamma(x-L)}\right]\cos(my).}
$$

It is an asymptotic formula: at $x=0$ the remaining mismatch is of order $A(\gamma L)^2$. Expanding the eastern exponential as well gives the familiar leading [Sverdrup balance](../../../../sverdrup-balance.md) interior plus western correction,

$$
\psi\simeq\frac{F_0}\beta\left[(x-L)+Le^{-x/\delta_W}\right]\cos(my),\qquad \delta_W=\frac r\beta.
$$

**Printed inequality.** The original PDF explicitly has $\lambda^{-1}\gg L$ as well as $\gamma^{-1}\gg L$. The first sign is reversed for the requested small-friction limit. This can also be disproved directly: if $\lambda L=0.02$ and $\gamma L=0.01$, the printed approximate bracket at the western wall is $1-0.01-e^{-0.01}\simeq-4.98\times10^{-5}$, while at the eastern wall it is $-0.01e^{-0.02}\simeq-0.00980$. The latter is of the same order as the retained basin-scale signal, violating the boundary condition at leading order. The exact expression above remains available without imposing the erroneous inequalities.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
