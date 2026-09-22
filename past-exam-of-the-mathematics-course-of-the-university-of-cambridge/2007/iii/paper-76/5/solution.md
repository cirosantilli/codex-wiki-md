<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $\boldsymbol\tau$ for the [Kirchhoff stress tensor](../../../../../kirchhoff-stress-tensor.md) and $S$ for the [second Piola-Kirchhoff stress tensor](../../../../../second-piola-kirchhoff-stress-tensor.md). Since $\boldsymbol\tau=FSF^T$ and $\dot F=LF$ for the [velocity gradient](../../../../../velocity-gradient.md),

$$
\dot{\boldsymbol\tau}=L\boldsymbol\tau+\boldsymbol\tau L^T+F\dot SF^T.
$$

Therefore the [upper-convected rate as a stress push-forward](../../../../../upper-convected-rate-as-a-stress-push-forward.md) is

$$
\boxed{\frac{\delta\boldsymbol\tau}{\delta t}=\dot{\boldsymbol\tau}-L\boldsymbol\tau-\boldsymbol\tau L^T=F\dot SF^T.}
$$

For the [simple shear flow](../../../../../simple-shear-flow.md), put $\gamma=f_{,2}$ and $g=\dot\gamma$. The [velocity gradient](../../../../../velocity-gradient.md) and [rate-of-strain tensor](../../../../../strain-rate-tensor.md) are

$$
L=\begin{pmatrix}0&g&0\\0&0&0\\0&0&0\end{pmatrix},\qquad D=\frac12\begin{pmatrix}0&g&0\\g&0&0\\0&0&0\end{pmatrix}.
$$

Their [upper-convected derivative](../../../../../upper-convected-derivative.md) gives

$$
\frac{\delta D}{\delta t}=\begin{pmatrix}-g^2&\dot g/2&0\\\dot g/2&0&0\\0&0&0\end{pmatrix}.
$$

Denote the symmetric extra stress by $E=\sigma^d$, and the relaxation time by $\tau_r$ to distinguish it from $\boldsymbol\tau$. The [Oldroyd-B model](../../../../../oldroyd-b-model.md) in the question becomes

$$
\begin{aligned}
\dot E_{11}-2gE_{12}+E_{11}/\tau_r&=-2\mu_rg^2,\\
\dot E_{12}-gE_{22}+E_{12}/\tau_r&=\mu g/\tau_r+\mu_r\dot g,\\
\dot E_{22}+E_{22}/\tau_r&=0,\qquad\dot E_{33}+E_{33}/\tau_r=0,\\
\dot E_{13}-gE_{23}+E_{13}/\tau_r&=0,\qquad\dot E_{23}+E_{23}/\tau_r=0.
\end{aligned}
$$

For the steady constitutive response, $E_{22}=E_{33}=E_{13}=E_{23}=0$, $E_{12}=\mu g$ and $E_{11}=2(\mu-\mu_r)\tau_rg^2$. Hence

$$
\boxed{\sigma_{11}=-p+2(\mu-\mu_r)\tau_rg^2,\quad\sigma_{12}=\mu g,\quad\sigma_{22}=\sigma_{33}=-p,\quad\sigma_{13}=\sigma_{23}=0.}
$$

A constant imposed shear rate can still have startup transients; these values describe the steady response.

For circular [Couette flow](../../../../../couette-flow.md) $v(r)e_\theta$, the [velocity gradient](../../../../../velocity-gradient.md) in the orthonormal polar basis $(e_r,e_\theta)$ is

$$
L=\begin{pmatrix}0&-v/r\\v'&0\end{pmatrix}.
$$

For completeness, in fixed Cartesian coordinates let $\omega(r)=v(r)/r$ and $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$. Then $v=\omega Jx$ and $L=\omega J+(\omega'/r)(Jx)\otimes x$. Along a particle, the polar basis rotates at angular speed $\omega$. Its contribution to the [material derivative](../../../../../material-derivative.md) cancels the rigid-rotation part of $L$ in the [upper-convected derivative](../../../../../upper-convected-derivative.md). The [rotating-frame reduction of circular viscoelastic shear](../../../../../rotating-frame-reduction-of-circular-viscoelastic-shear.md) therefore leaves

$$
L_{\rm eff}=\begin{pmatrix}0&0\\v'-v/r&0\end{pmatrix}.
$$

The flow direction is now $e_\theta$ and the gradient direction is $e_r$. With $g=v'-v/r$, the same simple-shear constitutive calculation gives

$$
\boxed{\sigma_{rr}=-p,\qquad\sigma_{r\theta}=\mu g,\qquad\sigma_{\theta\theta}=-p+2(\mu-\mu_r)\tau_rg^2.}
$$

Angular [force balance](../../../../../force-balance.md) implies $r^2\mu g$ is constant. Integrating $v'-v/r\propto r^{-2}$ gives $v=Ar+B/r$. With $v(a)=V_a$ and $v(b)=0$,

$$
B=\frac{V_aab^2}{b^2-a^2},\qquad A=-\frac B{b^2},\qquad g=-\frac{2B}{r^2}.
$$

The radial [force balance](../../../../../force-balance.md) is $-p'-2(\mu-\mu_r)\tau_rg^2/r=0$. Thus the [inertialess Oldroyd-B circular Couette pressure](../../../../../inertialess-oldroyd-b-circular-couette-pressure.md) is

$$
\boxed{p(r)=p_0+\frac{2(\mu-\mu_r)\tau_r}{r^4}\left(\frac{V_aab^2}{b^2-a^2}\right)^2.}
$$

The constant $p_0$ is fixed by a pressure or normal-traction boundary condition.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
