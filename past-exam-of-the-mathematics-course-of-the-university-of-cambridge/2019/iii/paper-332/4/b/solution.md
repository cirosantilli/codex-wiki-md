<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With both [ice accumulation](../../../../../../ice-accumulation.md) and [ice ablation](../../../../../../ice-ablation.md) removed, the equation is $h_t+x^{-1}(xDh^3)_x=0$ and the conserved volume is $V_0=2\pi\cos\alpha\,M$, where $M=\int_0^{x_N}xh\,dx$.

If the thickness and extent scales are $H(t)$ and $X(t)$, [mass conservation](../../../../../../mass-conservation.md) gives $HX^2\sim M$, while the flow equation gives $H/t\sim DH^3/X$. Therefore $X\propto t^{1/5}$ and $H\propto t^{-2/5}$. Set $h=\tau^{-2/5}f(\xi)$, $\xi=x\tau^{-1/5}$, with a possible virtual time origin $\tau=t+t_0$. The [similarity solution](../../../../../../similarity-solution.md) satisfies

$$
-\frac25 f-\frac15\xi f'+\frac D\xi(\xi f^3)'=0.
$$

Integration and regular zero total flux at the apex give $D\xi f^3=\xi^2f/5$, hence the positive profile is

$$
\boxed{h(x,\tau)=\sqrt{\frac{x}{5D\tau}},\qquad 0<x<x_N(\tau),}
$$

with dry bed beyond the front. Volume normalization gives

$$
M=\frac{2x_N^{5/2}}{5\sqrt{5D\tau}},
$$

so the [volume-conserving conical ice-current similarity solution](../../../../../../volume-conserving-conical-ice-current-similarity-solution.md) has

$$
\boxed{x_N=\left(\frac{125}{4}DM^2\tau\right)^{1/5}=\left(\frac{125g\sin\alpha\,V_0^2\tau}{48\pi^2\nu\cos^2\alpha}\right)^{1/5},\qquad h_N=\sqrt{\frac{x_N}{5D\tau}}.}
$$

The terminus has finite thickness and is a [shock wave](../../../../../../shock-wave.md) in the gravity-only [kinematic wave](../../../../../../kinematic-wave.md) equation. The [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md) gives $\dot x_N=q_N/h_N=Dh_N^2=x_N/(5\tau)$, exactly agreeing with the similarity extent. The characteristic speed behind the front is $3Dh_N^2$, larger than its speed, while the dry-bed characteristic speed is zero, so the front is compressive and gives an [entropy solution](../../../../../../entropy-solution.md).

This solution describes the long-time spreading, rather than exactly matching the earlier steady profile at the instant snowfall stops. The initial transient can be described by the [characteristic transformation for conical ice drainage](../../../../../../characteristic-transformation-for-conical-ice-drainage.md): with starting point $s$, put $K(s)=s^{1/3}h_s(s)$; then

$$
h(x,t)x^{1/3}=K(s),\qquad x^{5/3}=s^{5/3}+5DK(s)^2t
$$

where characteristics remain smooth. Subsequent crossings are resolved by the same conservation and entropy conditions. Restoring the neglected local pressure gradient would smooth the idealized front.

<a id="4/b/image-steady-accumulation-profile-and-volume-conserving-spreading-on-a-cone"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-332-conical-ice.png)

**[Figure 2](#4/b/image-steady-accumulation-profile-and-volume-conserving-spreading-on-a-cone). Steady accumulation profile and volume-conserving spreading on a cone**. The steady ice cap ends at three halves of the snowline distance. After accumulation and ablation cease, the long-time gravity-only similarity profile spreads outward and has a finite-thickness front. Both panels use the same conserved ice volume.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
