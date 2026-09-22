<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Keep the prescribed outer slip [velocity](../../../../../velocity.md) fixed when perturbing the [unsteady Prandtl equation](../../../../../unsteady-prandtl-equation.md). Cancelling the base equation and retaining terms linear in the disturbance gives the [linearized unsteady Prandtl equation](../../../../../linearized-unsteady-prandtl-equation.md)

$$
\tilde u_t+U\tilde u_x+V\tilde u_y+U_x\tilde u+U_y\tilde v
=\tilde u_{yy},\qquad
\tilde u_x+\tilde v_y=0.
$$

The [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) supplies $\tilde u=\tilde v=0$ at the wall; the fixed outer [velocity](../../../../../velocity.md) supplies $\tilde u\to0$ at infinity. There is no prescribed zero normal-velocity disturbance at infinity: a finite displacement-related value is permitted.

With the frozen parallel profile $U=U(y)$, $V=0$, the coefficients are invariant under translations in $x$ and $t$. [Normal modes](../../../../../normal-mode.md) therefore separate those variables. For the mode convention used here the equations are

$$
i\alpha(U-c)u+U'v=u'',\qquad i\alpha u+v'=0.
$$

Eliminate $u=-v'/(i\alpha)$ to obtain the [Prandtl normal-mode equation](../../../../../prandtl-normal-mode-equation.md)

$$
\boxed{v'''=i\alpha[(U-c)v'-U'v]},\qquad
v(0)=v'(0)=0,\quad v'(\infty)=0,
$$

with a bounded far-field $v$. Requiring $v(\infty)=0$ would incorrectly eliminate the proposed outer profile. For real $U$ and real $\alpha$, complex conjugation of the equation and its [boundary conditions](../../../../../boundary-condition.md) replaces $(\alpha,c,v)$ by $(-\alpha,c^*,v^*)$. This proves the stated [eigenvalue](../../../../../eigenvalue.md) symmetry. The paired modes have the same temporal [growth rate](../../../../../growth-rate.md) $\alpha\operatorname{Im}c$, so choosing positive [wavenumber](../../../../../wavenumber.md) loses no real physical disturbance.

Here the prescribed parallel profile is a local frozen-coefficient model. A nontrivial arbitrary $U(y)$ with $V=0$ and constant outer slip is not generally an exact steady solution of the unforced [unsteady Prandtl equation](../../../../../unsteady-prandtl-equation.md); its base equation would require $U''=0$. The following stability calculation uses the simplifying local model stipulated for the mode analysis.

Set $c_0=U_c=U(y_c)$. Away from the critical point the dominant equation is $(U-c_0)v_0'-U'v_0=0$, whose solutions are multiples of $U-c_0$. Choosing the coefficient to be zero below $y_c$ and one above it satisfies the wall and tangential far-field conditions. The choice $c_0=U_c$ makes $v_0$ continuous across the joining point; $U'(y_c)=0$ also makes its first [derivative](../../../../../derivative.md) continuous. Its second [derivative](../../../../../derivative.md) jumps. Thus it is a valid leading outer solution away from $y_c$, but viscosity must smooth the join in a [critical layer in a shear flow](../../../../../critical-layer-in-a-shear-flow.md).

Near the join, $U-c_0\sim(y-y_c)^2/2$. If the layer width is $\ell$, matching gives $v=O(\ell^2)$. The advection side of the mode equation scales as $\alpha\ell^3$ and $v'''$ scales as $\ell^{-1}$. Balance gives $\ell^4\sim\alpha^{-1}=\varepsilon/k$. Equivalently, the [eigenvalue](../../../../../eigenvalue.md) correction $\varepsilon^{1/2}c_1$ balances $(y-y_c)^2$, so the [quarter-power critical layer](../../../../../prandtl-critical-layer-at-a-stationary-shear-profile.md) has

$$
\boxed{p=\frac14,\qquad q=\frac12},\qquad
y-y_c=\varepsilon^{1/4}Y,\quad v=\varepsilon^{1/2}w(Y)+\cdots.
$$

Substitution, retaining the leading terms and cancelling their common factor, gives

$$
\boxed{kYw-k\left(\frac{Y^2}{2}-c_1\right)w_Y=iw_{YYY}}.
$$

At order $\varepsilon^{1/2}$ outside the layer,

$$
(U-c_0)v_1'-U'v_1=c_1v_0'.
$$

A solution consistent with the chosen lower branch and the wall conditions is $v_1=0$ below the join. Above it a particular solution is $v_1=-c_1$; a multiple of $U-c_0$ represents an arbitrary amplitude renormalization and may be set to zero. Matching consequently requires

$$
\boxed{w\to0\quad(Y\to-\infty),\qquad
w-\left(\frac{Y^2}{2}-c_1\right)\to0\quad(Y\to+\infty)}.
$$

The corresponding [derivatives](../../../../../derivative.md) match as $w_Y\sim Y$, $w_{YY}\to1$ on the positive side and as zero on the negative side. The matching statements require that growing homogeneous corrections be absent.

To symmetrize these different end conditions and remove $k$ and $i$, choose

$$
a=(ik)^{1/4}=k^{1/4}e^{i\pi/8},\qquad
z=aY,\quad C=a^2c_1,\quad
W=2a^2w-\left(\frac{z^2}{2}-C\right).
$$

The polynomial $A(z)=z^2/2-C$ is itself a solution of the transformed homogeneous equation. Direct substitution, using $a^4=ik$, gives

$$
\boxed{W_{zzz}-\left(\frac{z^2}{2}-C\right)W_z+zW=0},
\qquad W\mp\left(\frac{z^2}{2}-C\right)\to0\quad(z\to\pm\infty).
$$

The [derivative](../../../../../derivative.md) is third order, as required by the original mode equation. Initially the two ends are along the rotated rays $z=aY$ with real $Y$. Continuing them to the real $z$ axis is compatible with the asymptotic end conditions: the decreasing homogeneous correction behaves exponentially as $\exp[-z^2/(2\sqrt2)]$ and still decreases throughout the rotation from angle $\pi/8$ to zero. Thus the supplied real-axis spectral normalization uses the same recessive conditions; a complex coordinate change should not be mistaken for a real stretching alone.

For each supplied real [eigenvalue](../../../../../eigenvalue.md) $C_n=(4n+7)/\sqrt2$, the phase-speed correction is

$$
c_1=k^{-1/2}e^{-i\pi/4}C_n,\qquad
\operatorname{Im}c=-\frac{C_n}{\sqrt{2k}}\varepsilon^{1/2}+o(\varepsilon^{1/2}).
$$

The mode factor has temporal magnitude $e^{\alpha\operatorname{Im}c\,t}$. Therefore

$$
\boxed{\gamma_n=\alpha\operatorname{Im}c
=-\frac{4n+7}{2}\sqrt\alpha+o(\sqrt\alpha)}.
$$

Among the listed indices, $n=-2$ gives positive growth $\gamma\sim\sqrt\alpha/2$; $n=-1,1,2,\ldots$ give decay. Hence the frozen non-monotone flow has [high-wavenumber instability of a non-monotone Prandtl layer](../../../../../high-wavenumber-instability-of-a-non-monotone-prandtl-layer.md), with arbitrarily rapid linear growth as the positive [wavenumber](../../../../../wavenumber.md) increases. The normal-mode calculation demonstrates [linear instability](../../../../../linear-instability.md); it is not by itself a claim about the final nonlinear state.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
