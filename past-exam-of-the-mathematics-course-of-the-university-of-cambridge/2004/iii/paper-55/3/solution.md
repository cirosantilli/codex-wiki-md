<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use units $c=1$, signature $(+---)$, and the weak-field metric $g_{ab}=\eta_{ab}+h_{ab}$. Define the [trace-reversed metric perturbation](../../../../../trace-reversed-metric-perturbation.md) by $\bar h_{ab}=h_{ab}-\eta_{ab}h/2$, with $h=\eta^{ab}h_{ab}$. In the [Lorenz gauge in linearized gravity](../../../../../lorenz-gauge-in-linearized-gravity.md), $\partial^a\bar h_{ab}=0$, the sign convention of Q2 gives

$$
G^{(1)}_{ab}=\frac12\Box\bar h_{ab},\qquad
\Box\bar h_{ab}=-16\pi G T_{ab}.
$$

For completeness, the linearized [Ricci tensor](../../../../../ricci-tensor.md) in this convention is

$$
R^{(1)}_{ab}=\frac12\left(\Box h_{ab}+\partial_a\partial_bh-\partial_c\partial_ah^c{}_b-\partial_c\partial_bh^c{}_a\right).
$$

Substituting the Lorenz condition $\partial_ch^c{}_b=\partial_bh/2$ and trace reversing gives the stated [Einstein tensor](../../../../../einstein-tensor.md). For a stationary source, $\Box=-\nabla^2$, so $\nabla^2\bar h_{ab}=16\pi G T_{ab}$.

Keep the monopole terms of order $\epsilon=GM/R$ and the leading term linear in the rotation rate. Since $\Omega R=O(\epsilon^{1/2})$, the latter metric term is of order $\epsilon\Omega R=O(\epsilon^{3/2})$ on the shell. Thus it would disappear from a strictly order-$\epsilon$ truncation; the requested approximation must retain the leading rotation correction as well. Terms $T_{ij}=\rho v_iv_j$ generate metric corrections of order $\epsilon(\Omega R)^2=O(\epsilon^2)$ and are neglected. Corrections to four-velocity normalization and the supporting shell stresses affect the omitted higher orders. To retained order,

$$
T_{00}=\rho,\qquad T_{0i}=-\rho v_i,\qquad
\mathbf v=\boldsymbol\Omega\times\mathbf x,\quad\boldsymbol\Omega=\Omega\widehat{\mathbf z}.
$$

The minus sign in $T_{0i}$ comes from lowering its spatial index; using $T^{0i}$ in its place would reverse the dragging direction.

The scalar Poisson solution regular at the centre and vanishing at spatial infinity is $\bar h_{00}=-4GM/r$ outside the shell and $\bar h_{00}=-4GM/R=-4\epsilon$ inside. Continuity and the derivative jump $\bar h_{00}'(R^+)-\bar h_{00}'(R^-)=4GM/R^2$ verify the density $M\delta(r-R)/(4\pi R^2)$. Also $\bar h_{ij}=0$ at this order. Undoing trace reversal gives

$$
h_{00}=\frac12\bar h_{00}=-2\epsilon,\qquad h_{ij}=\frac12\delta_{ij}\bar h_{00}=-2\epsilon\delta_{ij}.
$$

Comparing with the scalar parts of the interior line element yields **$A=-\epsilon$ and $C=\epsilon$**.

For the mass-current contribution write

$$
\bar h_{0i}=F(r)(\widehat{\mathbf z}\times\widehat{\mathbf r})_i.
$$

Each nonzero angular component is a degree-one [spherical harmonic](../../../../../spherical-harmonic.md). The supplied [Laplacian](../../../../../laplacian.md) eigenvalue therefore gives

$$
F''+\frac2rF'-\frac2{r^2}F=-\frac{4GM\Omega}{R}\delta(r-R).
$$

Away from the shell, the two radial solutions are $r$ and $r^{-2}$. Regularity at $r=0$ and decay at infinity select $F_{\rm in}=ar$ and $F_{\rm out}=b/r^2$. Continuity at $R$ requires $b=aR^3$, and integrating the [differential equation](../../../../../differential-equation-split.md) across the shell gives

$$
F'(R^+)-F'(R^-)=-3a=-\frac{4GM\Omega}{R}.
$$

Thus $a=4GM\Omega/(3R)=\omega$, with $F_{\rm in}=\omega r$. Trace reversal leaves mixed components unchanged, so $h_{0i}=\omega(\widehat{\mathbf z}\times\mathbf x)_i=\omega(-y,x,0)_i$. The paper writes $g_{0i}=-B_i$, giving the [frame dragging inside a slowly rotating spherical shell](../../../../../frame-dragging-inside-a-slowly-rotating-spherical-shell.md)

$$
\boxed{-A=C=\epsilon,\qquad\mathbf B=\omega(y,-x,0),\qquad\omega=\frac{4\epsilon\Omega}{3}.}
$$

This dipole matching is valid throughout $r<R$; it does not assume the observation point is very close to the centre. The stationary current is divergence-free, so this solution also satisfies the Lorenz gauge. The exterior result is $h_{0i}=2G(\mathbf J\times\mathbf x)_i/r^3$, where the thin shell has $\mathbf J=(2/3)MR^2\boldsymbol\Omega$, providing a check on the coefficient.

To identify the freely falling frames inside, let $\mathcal R_z(\theta)$ be the ordinary spatial rotation by angle $\theta$. Define the [inertial coordinates inside a slowly rotating spherical shell](../../../../../inertial-coordinates-inside-a-slowly-rotating-spherical-shell.md) by

$$
T=(1-\epsilon)t,\qquad\mathbf X=(1+\epsilon)\mathcal R_z(-\omega t)\mathbf x.
$$

Differentiating and dropping $\epsilon^2$, products beyond the retained rotation order, and $\omega^2$ gives

$$
dT^2-d\mathbf X^2=(1-2\epsilon)dt^2-(1+2\epsilon)d\mathbf x^2+2(\boldsymbol\omega\times\mathbf x)\cdot d\mathbf x\,dt,
$$

which is precisely the interior metric. Thus the retained interior [curvature](../../../../../curvature.md) is zero, despite its nontrivial relation to the nonrotating coordinates anchored at infinity. [Timelike geodesics](../../../../../timelike-geodesic.md) in these local inertial coordinates are straight lines $\mathbf X=\mathbf X_0+\mathbf V T$, with $|\mathbf V|<1$. In the original coordinates this is

$$
\mathbf x(t)=\frac1{1+\epsilon}\mathcal R_z(\omega t)\{\mathbf X_0+(1-\epsilon)\mathbf Vt\},
$$

understood to the same perturbative order. Their coordinate equation is $d^2\mathbf x/dt^2=2\boldsymbol\omega\times d\mathbf x/dt$ to first rotation order. There is no interior Newtonian acceleration from the constant potential; the velocity-dependent term is the apparent Coriolis term relative to the locally dragged inertial axes.

A freely transported [gyroscope](../../../../../gyroscope.md) at rest in the interior to the retained order has constant spatial direction in the $\mathbf X$ frame, hence its direction in the original axes obeys $d\mathbf S/dt=\boldsymbol\omega\times\mathbf S$. **Local inertial axes precess in the same sense as the shell, at $\omega=(4\epsilon/3)\Omega$ relative to distant nonrotating axes.** This is the interior [Lense-Thirring precession](../../../../../lense-thirring-precession.md). For a weak shell the dragging is only a small fraction of its [angular velocity](../../../../../angular-velocity.md), not perfect corotation. It is compatible with the equivalence principle: rotation relative to distant axes is a comparison between frames, and local flatness at the retained order does not make that comparison vanish. Quadratic rotation terms, which would include centrifugal effects and additional [curvature](../../../../../curvature.md), are outside the requested leading approximation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
