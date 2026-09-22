<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a length $\ell$, velocity $U_s$, time $\ell/U_s$, and pressure $\rho U_s^2$, giving [Reynolds number](../../../../../../reynolds-number.md) $Re=U_s\ell/\nu$. Write perturbation velocity as $(u,v,w)$ and let $\mathcal L=\partial_t+U\partial_x-Re^{-1}\nabla^2$. Linearizing the incompressible [Navier-Stokes equations](../../../../../../navier-stokes-equation.md) gives

$$
\mathcal Lu+U'v=-p_x,\quad\mathcal Lv=-p_y,\quad\mathcal Lw=-p_z,\quad u_x+v_y+w_z=0.
$$

Taking the divergence gives $\nabla^2p=-2U'v_x$. Applying $\nabla^2$ to the wall-normal momentum equation and using

$$
\nabla^2(Uv_x)=U\nabla^2v_x+2U'v_{xy}+U''v_x
$$

then cancels the pressure derivatives and yields $\mathcal L\nabla^2v-U''v_x=0$. Define wall-normal [vorticity](../../../../../../vorticity.md) $\eta=u_z-w_x$. Applying $\partial_z$ to the streamwise equation minus $\partial_x$ to the spanwise equation gives $\mathcal L\eta=-U'v_z$.

For the assumed [normal modes](../../../../../../normal-mode.md), set $D=d/dy$ and $\kappa^2=\alpha^2+\beta^2$. The two equations become the [Orr-Sommerfeld equation](../../../../../../orr-sommerfeld-equation.md) and [Squire equation](../../../../../../squire-equation.md):

$$
\boxed{[(-i\omega+i\alpha U)(D^2-\kappa^2)-i\alpha U''-Re^{-1}(D^2-\kappa^2)^2]\widehat v=0,}
$$



$$
\boxed{[(-i\omega+i\alpha U)-Re^{-1}(D^2-\kappa^2)]\widehat\eta=-i\beta U'\widehat v.}
$$

At rigid no-slip walls the conditions are $\widehat v=D\widehat v=\widehat\eta=0$ for nonzero horizontal wavenumber.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
