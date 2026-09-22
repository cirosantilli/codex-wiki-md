<h1 id="36e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix the scaling constants as $U=A/z$, $\delta=Bz$, with $A=F/(\rho\nu)$ and $B=\nu\sqrt{\rho/F}$, so $AB^2=\nu$. The [Stokes streamfunction](../../../../../../stokes-streamfunction.md) is then $\psi=\nu zf(\eta)$. Write $g=f'/\eta$. Differentiation gives

$$
u_z=\frac Azg,\qquad u_r=\frac{AB}{z}\left(f'-\frac f\eta\right),\qquad \partial_ru_z=\frac A{Bz^2}g',\quad\partial_zu_z=-\frac A{z^2}(g+\eta g').
$$

Substitution in the boundary-layer equation, cancelling $A^2/z^3$, gives $-(f/\eta)g'-g^2=g''+g'/\eta$. Multiplication by $\eta^3$ therefore gives **the required similarity equation**

$$
\boxed{ff'-\eta(f'^2+ff'')=f'-\eta f''+\eta^2f'''.}
$$

Axis regularity requires zero radial velocity and a finite smooth axial velocity: choose the streamfunction gauge $f(0)=0$ and require $f(\eta)=c\eta^2+O(\eta^4)$. Equivalently $f'(0)=0$, $f'/\eta$ has a finite limit, and $(f'/\eta)'\to0$ at the axis. The constant $c$ is not specified in advance. In the quiescent ambient fluid require $f'/\eta\to0$ and $f'-f/\eta\to0$ as $\eta\to\infty$, so both velocity components vanish. The localized physical jet has finite axial volume flux, corresponding to finite $f(\infty)$.

Finally the prescribed force fixes the amplitude through the finite momentum-flux normalization

$$
\boxed{2\pi\int_0^\infty\frac{f'(\eta)^2}{\eta}\,d\eta=1.}
$$

The axis conditions express regularity rather than independently prescribed arbitrary derivatives; the far-field conditions express matching to the resting fluid, and the integral condition supplies the jet strength.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [36E](../../36e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
