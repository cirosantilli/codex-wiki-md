<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take the primitive state vector $\mathbf U=(\rho,p,u_x,u_y,u_z,B_x,B_y,B_z)^T$, with $\rho>0$. In the absence of gravity, the [ideal magnetohydrodynamic equations](../../../../../ideal-magnetohydrodynamic-equations.md) are first order: expanding the [material derivatives](../../../../../material-derivative.md), [pressure](../../../../../pressure.md) gradient and [Lorentz force](../../../../../lorentz-force.md) makes every term linear in a spatial derivative of $\mathbf U$, with coefficients depending on $\mathbf U$. Dividing [momentum](../../../../../momentum.md) balance by $\rho$ therefore gives a [quasilinear partial differential equation](../../../../../quasilinear-partial-differential-equation.md) system $\partial_t\mathbf U+A_i(\mathbf U)\partial_i\mathbf U=0$ with eight-by-eight matrices. The [solenoidal magnetic-field constraint](../../../../../solenoidal-magnetic-field-constraint.md) is an additional constraint on initial data; the [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) preserves it because the divergence of a curl vanishes.

For a one-dimensional [simple wave in magnetohydrodynamics](../../../../../simple-wave-in-magnetohydrodynamics.md), write $\mathbf U=\mathbf U(q(x,t))$ with a nonzero state-space tangent. Substitution gives $\mathbf U_q q_t+A_x\mathbf U_q q_x=0$. A nonconstant profile requires the tangent to be a right [eigenvector](../../../../../eigenvector.md) of $A_x$:

$$
A_x\mathbf U_q=v(q)\mathbf U_q,\qquad q_t+v(q)q_x=0.
$$

The [chain rule](../../../../../chain-rule.md) then gives **the wave-speed equation**:

$$
\boxed{v_t+v v_x=v_q(q_t+v q_x)=0.}
$$

This is the [Inviscid Burgers equation](../../../../../inviscid-burgers-equation.md), including the special case of constant $v$. Its [characteristic curves](../../../../../characteristic-curve.md) are $x=a+v_0(a)t$, with $v=v_0(a)$. As long as the mapping remains invertible,

$$
v_x=\frac{v_0'(a)}{1+t v_0'(a)}.
$$

Thus a region with $v_0'<0$ steepens: faster characteristics catch slower ones, and the first gradient catastrophe occurs at $t_*=-1/\min_a v_0'(a)$ when the minimum is negative. A genuinely nonlinear compressive [simple wave](../../../../../simple-wave.md) therefore forms a [shock wave](../../../../../shock-wave.md). Rarefactive profiles can spread instead; steepening is not inevitable for every initial profile.

To continue past this time, use [weak solutions](../../../../../weak-solution.md) of the conservative mass, [momentum](../../../../../momentum.md), [fluid total-energy equation](../../../../../fluid-total-energy-equation.md) and [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md). The [Rankine-Hugoniot conditions](../../../../../rankine-hugoniot-conditions.md) fix the jumps and shock velocity, while physical entropy production selects admissible [magnetohydrodynamic shocks](../../../../../magnetohydrodynamic-shock.md). Diffusive [shock wave](../../../../../shock-wave.md) layers are replaced by moving discontinuities, so their microscopic structure need not be explicitly resolved. In particular, the smooth adiabatic [pressure](../../../../../pressure.md) equation must be replaced by total-energy conservation when imposing the [ideal magnetohydrodynamic shock conditions](../../../../../ideal-magnetohydrodynamic-shock-conditions.md).

For the [Alfvén waves](../../../../../alfven-wave.md), impose the one-dimensional [solenoidal magnetic-field constraint](../../../../../solenoidal-magnetic-field-constraint.md), so $B_x$ is constant and $\delta B_x=0$. Put $\mathbf B_\perp=(B_y,B_z)$ and $c=v-u_x$. The transverse components of the [linearized ideal magnetohydrodynamic equations](../../../../../linearized-ideal-magnetohydrodynamic-equations.md) give

$$
-c\,\delta\mathbf u_\perp-\frac{B_x}{\mu_0\rho}\delta\mathbf B_\perp=0,\qquad
-c\,\delta\mathbf B_\perp-B_x\delta\mathbf u_\perp=0.
$$

The longitudinal [momentum](../../../../../momentum.md) equation additionally gives $\delta p+\mathbf B_\perp\cdot\delta\mathbf B_\perp/\mu_0=0$. The Alfvén [eigenvectors](../../../../../eigenvector.md) have $\delta\rho=\delta p=\delta u_x=0$, hence their transverse polarization is perpendicular to $\mathbf B_\perp$. For $s=\pm1$, their speed and explicit right [Alfvén characteristic eigenvectors](../../../../../alfven-characteristic-eigenvector.md) are

$$
\boxed{v_s=u_x+s\frac{B_x}{\sqrt{\mu_0\rho}},\qquad
r_s=\begin{pmatrix}0\\0\\0\\h_y\\h_z\\0\\-s\sqrt{\mu_0\rho}\,h_y\\-s\sqrt{\mu_0\rho}\,h_z\end{pmatrix},\quad B_yh_y+B_zh_z=0.}
$$

For $\mathbf B_\perp\ne0$ one may choose $(h_y,h_z)=(B_z,-B_y)$, up to a nonzero scalar factor. If $\mathbf B_\perp=0$, either transverse polarization is allowed and this characteristic speed is degenerate. These expressions describe the two propagating Alfvén branches for $B_x\ne0$; if $B_x=0$, they coalesce with advected, nonpropagating transverse disturbances.

Integrating along an Alfvén [simple wave](../../../../../simple-wave.md) leaves $\rho,p,u_x,B_x$ unchanged and gives $d\mathbf u_\perp=-s\,d\mathbf B_\perp/\sqrt{\mu_0\rho}$ and $\mathbf B_\perp\cdot d\mathbf B_\perp=0$. Consequently **the finite-amplitude [nonlinear Alfvén wave](../../../../../nonlinear-alfven-wave.md) relations** are

$$
\boxed{f_1=C_y-\frac{s f_3}{\sqrt{\mu_0\rho}},\qquad f_2=C_z-\frac{s f_4}{\sqrt{\mu_0\rho}},\qquad f_3^2+f_4^2=B_\perp^2=\text{constant},\qquad v=v_s.}
$$

The constant-magnitude condition is essential: otherwise a varying [magnetic pressure](../../../../../magnetic-pressure.md) would drive longitudinal compression. An arbitrary smooth phase profile gives an explicit family, $f_3=B_\perp\cos\Theta(x-v_st)$ and $f_4=B_\perp\sin\Theta(x-v_st)$, with $f_1,f_2$ as above. Direct substitution in the transverse [momentum](../../../../../momentum.md) and [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) gives $(u_x-v_s)\mathbf u_\perp'=B_x\mathbf B_\perp'/(\mu_0\rho)$ and $(u_x-v_s)\mathbf B_\perp'=B_x\mathbf u_\perp'$, confirming the solution without relying on the [eigenvector](../../../../../eigenvector.md) argument. Longitudinal [momentum](../../../../../momentum.md) holds because $p+B_\perp^2/(2\mu_0)$ is constant. The speed $v_s$ is independent of amplitude along this family: **these [linearly degenerate characteristic fields](../../../../../linearly-degenerate-characteristic-field.md) translate without steepening**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 314](../../paper-314-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
