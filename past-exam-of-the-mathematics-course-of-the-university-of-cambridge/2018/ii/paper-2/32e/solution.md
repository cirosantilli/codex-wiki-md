<h1 id="32e/solution">Solution</h1>

↑ **Parent:** [32E](../32e.md)

The equilibrium equations give $y=0$ and $x-x^3=0$, so the fixed points are

$$
\boxed{(0,0),\qquad(1,0),\qquad(-1,0).}
$$

The Jacobian is

$$
J(x,0)=
\begin{pmatrix}
0&1\\
1-3x^2&\varepsilon(1-\alpha x^2)
\end{pmatrix}.
$$

At the origin its determinant is $-1$, so the origin is a [saddle equilibrium](../../../../../saddle-equilibrium.md). At either of the other points the determinant is two and the trace is $\varepsilon(1-\alpha)$. For small positive $\varepsilon$, they are unstable foci when $\alpha<1$ and stable foci when $\alpha>1$; at $\alpha=1$ the linearization is nonhyperbolic. When $\varepsilon=0$, each is a [center equilibrium](../../../../../center-equilibrium.md).

For $\varepsilon=0$, the system is [Hamiltonian](../../../../../hamiltonian.md) with

$$
\boxed{H(x,y)=\frac12y^2-\frac12x^2+\frac14x^4,}
$$

because $\dot x=H_y$ and $\dot y=-H_x$. Its [conservative planar phase portrait](../../../../../conservative-planar-phase-portrait.md) has two wells centered at $(\pm1,0)$, a saddle at the origin, periodic level curves around each center for $-1/4<H<0$, two homoclinic loops on $H=0$, and outer periodic curves surrounding both wells for $H>0$.

For positive small $\varepsilon$,

$$
\dot H=H_x\dot x+H_y\dot y
=\varepsilon(1-\alpha x^2)y^2.
$$

On the unperturbed level $H=H_0$,

$$
y^2=2H_0+x^2-\frac12x^4.
$$

The upper and lower halves contribute equally because $dt=dx/y$. Hence the [energy balance for the weakly perturbed double-well oscillator](../../../../../energy-balance-for-the-weakly-perturbed-double-well-oscillator.md) is

$$
\Delta H
=2\varepsilon\int_{x_1}^{x_2}
(1-\alpha x^2)
\sqrt{2H_0+x^2-\frac12x^4}dx+O(\varepsilon^2),
$$

so one may take

$$
\boxed{F(x;\alpha,H_0)=
2(1-\alpha x^2)
\sqrt{2H_0+x^2-\frac12x^4}.}
$$

For the right homoclinic loop, $H_0=0$, $x_1=0$, and $x_2=\sqrt2$. Its persistence requires

$$
0=\int_0^{\sqrt2}(1-\alpha x^2)x
\sqrt{1-x^2/2}dx.
$$

The substitution $u=1-x^2/2$ gives

$$
\int_0^{\sqrt2}x\sqrt{1-x^2/2}dx=\frac23,
\qquad
\int_0^{\sqrt2}x^3\sqrt{1-x^2/2}dx=\frac8{15}.
$$

Thus the [homoclinic balance for the weakly perturbed double-well oscillator](../../../../../homoclinic-balance-for-the-weakly-perturbed-double-well-oscillator.md) occurs at

$$
\boxed{\alpha=\frac{2/3}{8/15}=\frac54.}
$$

The left loop gives the same condition by symmetry.

For an orbit surrounding one center, the corresponding balance ratio tends to $\alpha=1$ as the orbit shrinks to the center and to $\alpha=5/4$ as it approaches the homoclinic loop. The [single-well periodic orbit range for the weakly perturbed double-well oscillator](../../../../../single-well-periodic-orbit-range-for-the-weakly-perturbed-double-well-oscillator.md) is therefore

$$
\boxed{1<\alpha<\frac54.}
$$

## ↑ Ancestors (10)

1. [32E](../32e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
