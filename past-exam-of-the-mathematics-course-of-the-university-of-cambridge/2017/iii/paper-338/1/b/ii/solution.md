<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [star](../../../../../../../star.md) of [declination](../../../../../../../declination.md) $\delta=\theta$ crosses the [zenith](../../../../../../../zenith.md). Its direction rotates around the [celestial pole](../../../../../../../celestial-pole.md) at $\Omega_{\rm sid}$, but its actual [angular velocity](../../../../../../../angular-velocity.md) on the [celestial sphere](../../../../../../../celestial-sphere.md) is $\Omega_{\rm sid}\cos\theta$. Consequently the small-angle crossing-gap estimate becomes

$$
\boxed{\phi_{\rm full}\simeq\frac{\pi\cos\theta}{\omega T_{\rm sid}},\qquad
\phi_{\rm radius}\simeq\frac{\pi\cos\theta}{2\omega T_{\rm sid}}.}
$$

For clarity, the factor $\cos\theta$ is the radius of the [star](../../../../../../../star.md)'s daily circle on a unit [celestial sphere](../../../../../../../celestial-sphere.md); it does not modify the sidereal [hour angle](../../../../../../../hour-angle.md) rate.

The estimate assumes the required slew is nearly $180^\circ$. A more exact ideal symmetric reacquisition calculation is possible. Let the endpoints have [hour angles](../../../../../../../hour-angle.md) $-H,+H$ and suppose $0<\theta<\pi/2$, $H$ small enough that both endpoints are above the [astronomical horizon](../../../../../../../astronomical-horizon.md). The horizontal direction components are $n=\sin\theta\cos\theta(1-\cos H)$ and $w=\pm\cos\theta\sin H$. Their shortest [azimuth](../../../../../../../azimuth.md) separation is

$$
\Delta\eta(H)=2\arctan\!\left(\frac{\cot(H/2)}{\sin\theta}\right).
$$

The minimum ideal gap satisfies $2H\Omega_{\rm az}/\Omega_{\rm sid}=\Delta\eta(H)$; its angular separation is $\phi_{\rm full}=2\arcsin(\cos\theta\sin H)$. Expanding for a fast drive gives the boxed expression. At an equatorial site $\Delta\eta=\pi$ exactly. At a geographic pole the direction with $\delta=\theta$ is stationary, so the crossing argument is inapplicable and the limit is zero. A full near-[zenith](../../../../../../../zenith.md) rate-limited footprint still requires specifying the trajectory and drive model.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
