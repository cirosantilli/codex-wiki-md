<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Reflection symmetry gives $\Phi_z(R,0)=0$. In a vertically stable [thin disk](../../../../../thin-disk.md), expand the vertical force as $\Phi_z(R,z)=\Omega_z^2z+O(z^3)$, where $\Omega_z^2=\Phi_{zz}(R,0)$ is the [vertical epicyclic frequency](../../../../../vertical-epicyclic-frequency.md) squared. For local [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) and height-independent [isothermal sound speed](../../../../../isothermal-sound-speed.md), $p=c_s^2\rho$ and

$$
c_s^2\rho_z=-\rho\Omega_z^2z.
$$

Thus $\rho=\rho_0\exp[-z^2/(2H^2)]$ with $H=c_s/\Omega_z$. Integrating the [pressure](../../../../../pressure.md) and [mass density](../../../../../density.md) through the disk gives the [vertically integrated pressure of an isothermal disk](../../../../../vertically-integrated-pressure-of-an-isothermal-disk.md):

$$
\boxed{P=c_s^2\Sigma=\Omega_z^2\Sigma H^2.}
$$

The force expansion is approximate in $H/R$, while $P=c_s^2\Sigma$ is exact for a height-independent sound speed.

In a nearly [Keplerian disk](../../../../../keplerian-disk.md), the vertical oscillation and radial [epicyclic motion](../../../../../epicyclic-motion.md) frequencies are close to the orbital frequency. The exact leading orbital differences are $\Omega-\Omega_z$ and $\Omega-\kappa$, so

$$
\Omega-\Omega_z=\frac{\Omega^2-\Omega_z^2}{\Omega+\Omega_z}\simeq\omega_1,\qquad
\Omega-\kappa=\frac{\Omega^2-\kappa^2}{\Omega+\kappa}\simeq\omega_2.
$$

Thus **$\omega_1$ is the nodal precession rate of a slightly tilted orbit, and $\omega_2$ is the apsidal precession rate of a slightly eccentric orbit**. Their signs distinguish prograde from retrograde [precession](../../../../../precession.md). This also agrees with the sign convention in the complex tilt: a freely precessing ring obeys $W_t=i\omega_1W$.

For exactly Keplerian motion, $\Omega_z=\kappa=\Omega$, so $\omega_1=\omega_2=0$ and $P/\Sigma=c_s^2$. In the local approximation, freeze the slowly varying coefficients and take $W,G\propto e^{i(kR-\omega t)}$. The [inviscid warp equations of a nearly Keplerian disk](../../../../../inviscid-warp-equations-of-a-nearly-keplerian-disk.md) become

$$
-i\omega\Sigma R^2\Omega W=\frac{ik}{R}G,\qquad
-i\omega G=\frac{ik}4PR^3\Omega W.
$$

Eliminating $G$ gives $\omega^2=k^2P/(4\Sigma)=k^2c_s^2/4$. Hence

$$
\boxed{\omega=\pm\frac12c_sk,\qquad v_{\mathrm{group}}=\pm\frac12c_s.}
$$

These are [bending waves of a Keplerian disk](../../../../../bending-wave-of-a-keplerian-disk.md), carrying changes in orbital tilt. The local approximation needs wavelength small compared with $R$; the secular thin-disk warp equations also describe the long-vertical-wavelength regime $H\ll\lambda\ll R$.

For a nonspinning hole, $a=0$ gives $\omega_1=0$. A steady [disk warp](../../../../../disk-warp.md) then satisfies $G_R=0$. The zero inner torque forces $G=0$ throughout, and the second warp equation, with positive $P$, forces $W_R=0$. The outer orientation fixes **$W(R)=W_\infty$ everywhere**. An apsidal precession term by itself therefore does not require a tilt warp.

For nonzero spin, set the time derivatives to zero. The two equations give

$$
G_R=-i\omega_1\Sigma R^3\Omega W,\qquad
G=i\frac{PR^3\Omega}{4\omega_2}W_R.
$$

Eliminating the internal [torque](../../../../../torque.md) yields

$$
\frac d{dR}\left(\frac{PR^3\Omega}{4\omega_2}W_R\right)+\omega_1\Sigma R^3\Omega W=0.
$$

Use $\omega_2=3\Omega/r$, $\omega_1=2a\Omega r^{-3/2}$, $\Omega^2R^3=GM$, and $P\simeq\Omega^2\Sigma H^2$. The first coefficient becomes $GM\Sigma H^2r/12$ and the second becomes $2aGM\Sigma r^{-3/2}$. Therefore

$$
\boxed{\frac d{dR}\left(\Sigma H^2r\frac{dW}{dR}\right)+24a\,r^{-3/2}\Sigma W=0.}
$$

This is the stationary [disk warp](../../../../../disk-warp.md) equation under the stated weak-precession approximations. The inner condition is $W_R(R_{\mathrm{in}})=0$ when its coefficient is finite and nonzero, because $G=iGM\Sigma H^2rW_R/12$.

Let $R_g=GM/c^2$, so $R=R_gr$, and impose $H=\epsilon R$, $\Sigma\propto R^{-3/4}$. Converting both radial derivatives carefully to $r$ and dividing out the common positive factor gives

$$
\frac d{dr}\left(r^{9/4}W_r\right)+\frac{24a}{\epsilon^2}r^{-9/4}W=0,
$$

or $W_{rr}+9W_r/(4r)+(24a/\epsilon^2)r^{-9/2}W=0$. For $a>0$, introduce

$$
x=\frac{4\sqrt{24a}}{5\epsilon}r^{-5/4}.
$$

Since $x_r$ is proportional to $r^{-9/4}$, the first-derivative term cancels exactly, leaving $W_{xx}+W=0$. Thus $W=A\cos x+B\sin x$.

The outer boundary $r\to\infty$ is $x\to0$, giving $A=W_\infty$. The specified inner-radius relation is exactly $x_{\mathrm{in}}=\pi$. The inner zero-torque condition $W_x(\pi)=0$ then gives $B=0$. Hence the [stationary bending warp of a Kerr disk](../../../../../stationary-bending-warp-of-a-kerr-disk.md) is

$$
\boxed{W(r)=W_\infty\cos\!\left[\pi\left(\frac{r_{\mathrm{in}}}{r}\right)^{5/4}\right].}
$$

The tilt magnitude is $\beta(r)=|W_\infty|\,|\cos x|$. Far out it tends to the imposed tilt. Moving inward, it decreases to zero at

$$
\boxed{r_{\mathrm{node}}=2^{4/5}r_{\mathrm{in}},}
$$

then grows again with opposite signed tilt, reaching $W(r_{\mathrm{in}})=-W_\infty$. All tilt vectors lie on the same line in the complex $W$ plane. Their azimuth is $\arg W_\infty$ outside the node and differs by $\pi$ inside; azimuth is undefined at the aligned node itself. The tilt vector remains smooth there. Thus this is an oscillatory standing bending warp, with equal outer and inner tilt magnitudes and reversed inner orientation, rather than monotone inner alignment.

The prescribed real inner radius assumes $a>0$: for $a<0$, its square root is not real, so that particular boundary prescription does not apply. With a separately chosen positive inner radius and negative spin, put $x=4\sqrt{24|a|}\,r^{-5/4}/(5\epsilon)$. The equation becomes $W_{xx}-W=0$, and the same outer tilt and zero inner torque give

$$
W(r)=W_\infty\frac{\cosh(x_{\mathrm{in}}-x)}{\cosh x_{\mathrm{in}}}.
$$

This negative-spin solution decreases smoothly toward the inner disk without a sign reversal. The specified positive-spin solution is the cosine profile above; the $a=0$ case is the flat solution already derived.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
