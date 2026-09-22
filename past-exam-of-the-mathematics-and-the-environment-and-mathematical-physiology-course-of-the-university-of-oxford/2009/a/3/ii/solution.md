<h1 id="a/3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take an arbitrary reference depth $h_0>0$, and select $u_0=(gSh_0/f)^{1/2}$ so the uniform reference flow balances drag and slope. Work with positive downstream [velocity](../../../../../velocity.md), so $u_*=\sqrt f\,u$ in the dimensional constitutive laws. Introduce the erosion and bedload scales

$$
E_0=\frac{bf^{3/2}u_0^3}{v_s^2},\qquad q_{b0}=\frac{\rho_wKf^{3/2}u_0^3}{\Delta\rho g}.
$$

Matching erosion with deposition, suspended [advection](../../../../../advection.md) with erosion, and bed storage with erosion gives respectively

$$
c_0=\frac{\rho_sbf^2u_0^4}{\gamma v_s^4},\qquad x_0=\frac{h_0c_0u_0}{\rho_sE_0}=\frac{h_0\sqrt f\,u_0^2}{\gamma v_s^2},\qquad t_0=\frac{(1-\phi)h_0}{E_0}.
$$

Use $h_0$ for the scales of $\eta$ and $s$ too, so $h=\eta-s$ survives unchanged. After dividing the balances by their matched scales, the parameters are

$$
\boxed{\epsilon=\frac{x_0}{u_0t_0}=\frac{c_0}{\rho_s(1-\phi)},\quad F=\frac{u_0}{\sqrt{gh_0}},\quad\delta=\frac{Sx_0}{h_0},\quad\beta=\frac{q_{b0}}{E_0x_0}=\frac{\rho_wK v_s^2}{\Delta\rho g b x_0}.}
$$

For example the [momentum](../../../../../momentum-split.md) balance divided by $gh_0/x_0$ has inertial prefactor $F^2$, surface-gradient term $-\eta_x$, and equal slope/drag prefactors $Sx_0/h_0=\delta$, because $fu_0^2=gSh_0$. The suspended balance has source $u^3-c/u$, and the bed balance has its negative with unit bed-time coefficient by the definition of $t_0$. These substitutions give the entire stated dimensionless system; $q_b=u^3$ is dimensionless bedload, with its dimensional scale already absorbed into $\beta$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
