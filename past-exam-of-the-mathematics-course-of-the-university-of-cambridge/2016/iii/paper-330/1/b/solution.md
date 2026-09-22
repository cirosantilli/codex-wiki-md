<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take a common constant [buoyancy frequency](../../../../../../buoyancy-frequency.md) $N$ and put $k=k_T>0$. Define $\eta$ to be vertical parcel [displacement](../../../../../../displacement.md); the [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) is $w=ikU_j\eta_j$. In either uniform region the exact [Taylor–Goldstein equation](../../../../../../taylor-goldstein-equation.md) gives

$$
\eta_j''+m_j^2\eta_j=0,\qquad m_j^2=\frac{N^2}{U_j^2}-k^2.
$$

No [WKB approximation](../../../../../../wkb-approximation.md) is needed. If the earlier $N(z)$ is genuinely nonconstant, the exact regional equation is instead $\eta_j''+[N(z)^2/U_j^2-k^2]\eta_j=0$; its fundamental solutions, not plane exponentials, must be used. For example, let $C_1(0)=1$, $C_1'(0)=0$, $S_1(0)=0$, $S_1'(0)=1$, and let $f_2$ be an outgoing upper solution. Then $\eta_1=h_0C_1+D S_1$, $\eta_2=A f_2$, with $D,A$ determined by $h_0C_1(H)+DS_1(H)=Af_2(H)$ and $U_1^2[h_0C_1'(H)+DS_1'(H)]=U_2^2Af_2'(H)$. This gives the exact arbitrary-profile field implicitly, while a simple angle-only coefficient requires further stratification assumptions.

Under the common constant-$N$ assumption, propagating incident [internal gravity waves](../../../../../../internal-wave.md) require

$$
\boxed{0<U_1<\frac Nk.}
$$

For co-directed upper flow, the outgoing propagating branch exists for $0<U_2<N/k$ and has $m_2>0$. The [radiation condition](../../../../../../radiation-condition.md) chooses $m_j>0$ because the laboratory vertical [group velocity](../../../../../../group-velocity.md) is positive on the negative [intrinsic frequency](../../../../../../intrinsic-frequency.md) branch. Define $\tan\theta_j=m_j/k$, so $\cos\theta_j=kU_j/N$.

At the [velocity](../../../../../../velocity.md) jump, the material-interface [jump conditions for stratified inviscid shear flow](../../../../../../jump-conditions-for-stratified-inviscid-shear-flow.md) require continuity of [displacement](../../../../../../displacement.md) and of [fluid pressure](../../../../../../fluid-pressure.md). Vertical [velocity](../../../../../../velocity.md) itself is generally discontinuous: $w_j=ikU_j\eta$. In terms of [displacement](../../../../../../displacement.md) the pressure is $p_j=U_j^2\eta_j'$. The [displacement impedance for an internal wave at a velocity jump](../../../../../../displacement-impedance-for-an-internal-wave-at-a-velocity-jump.md) is $Z_j=U_j^2m_j$. An upward incident component of complex [displacement](../../../../../../displacement.md) [amplitude](../../../../../../wave-amplitude.md) $I$ at $H$, a reflected component $RI$ and a transmitted component $TI$ therefore obey

$$
1+R=T,\qquad Z_1(1-R)=Z_2T.
$$

Consequently

$$
\boxed{R=\frac{Z_1-Z_2}{Z_1+Z_2},\qquad T=\frac{2Z_1}{Z_1+Z_2}.}
$$

For a one-pass incident [displacement](../../../../../../displacement.md) $h_0$, a real wave field is the imaginary part of

$$
\begin{aligned}
\eta_1(x,z)&=h_0e^{ikx}\left[e^{im_1z}+R e^{im_1(2H-z)}\right],&&0<z<H,\\
\eta_2(x,z)&=h_0T e^{i[kx+m_1H+m_2(z-H)]},&&z>H.
\end{aligned}
$$

The incident vertical-[displacement](../../../../../../displacement.md) [amplitude](../../../../../../wave-amplitude.md) is $h_0$, the reflected [amplitude](../../../../../../wave-amplitude.md) is $|R|h_0$ and the transmitted [amplitude](../../../../../../wave-amplitude.md) is $|T|h_0$; the sign of $R$ encodes a phase reversal. The other fields follow from $w=ikU\eta$, $u=-w'/(ik)$, $b=-N^2\eta$ and $p=U^2\eta'$. If a perfectly reflecting terrain boundary is enforced after the return wave arrives, replace the incident coefficient $h_0$ by $h_0/[1+Re^{2im_1H}]$. The one-pass [amplitudes](../../../../../../wave-amplitude.md) use the permitted neglect of repeated terrain reflections.

For common $N$, $Z_j=(N^2/k)\cos\theta_j\sin\theta_j$. The physical vertical-[displacement](../../../../../../displacement.md) transmission coefficient is therefore

$$
\boxed{\frac{\eta_{2,\mathrm{vertical}}}{h_0}=\frac{2\cos\theta_1\sin\theta_1}{\cos\theta_1\sin\theta_1+\cos\theta_2\sin\theta_2}=\frac{2\cos\theta_1\sin\theta_1}{\sin(\theta_1+\theta_2)\cos(\theta_1-\theta_2)}.}
$$

The printed coefficient has a different denominator and cannot be obtained for this standard [displacement](../../../../../../displacement.md) convention. For example, when $U_2=U_1$, there is no interface scattering and the vertical [amplitude](../../../../../../wave-amplitude.md) stays $h_0$, whereas the printed expression gives $h_0/\cos\theta_1$. A total [displacement](../../../../../../displacement.md) magnitude would instead be the vertical [amplitude](../../../../../../wave-amplitude.md) divided by $\cos\theta_2$; with unequal [velocities](../../../../../../velocity.md) it still does not give the printed expression. **The transmission formula needs an explicit correction or a different, presently unspecified [amplitude](../../../../../../wave-amplitude.md)/interface model.**

For $U_2>N/k$, choose $m_2=i\kappa$ with $\kappa=(k^2-N^2/U_2^2)^{1/2}$: the transmitted response decays as $e^{-\kappa(z-H)}$ and the same impedance equations give a complex $R,T$, with $|R|=1$. At $U_2=0$ the steady equation is singular. Oppositely directed upper flow formally supports propagating waves when $0<|U_2|<N/k$, but upward radiation then requires $m_2<0$ and signed $Z_2$; the positive-angle co-directed formula is not valid there. A real [velocity](../../../../../../velocity.md) jump can also have [Kelvin-Helmholtz instability](../../../../../../kelvin-helmholtz-instability.md), which is excluded from this formal steady scattering calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 330](../../../paper-330-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
