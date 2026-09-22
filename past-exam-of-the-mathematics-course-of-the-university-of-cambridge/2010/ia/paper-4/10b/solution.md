<h1 id="10b/solution">Solution</h1>

↑ **Parent:** [10B](../10b.md)

For the [inverse-square potential](../../../../../inverse-square-potential.md) $V(r)=-Q/r$, the [central force](../../../../../central-force.md) is $-V'(r)\hat r=-Q\hat r/r^2$. The transverse component of [acceleration in polar coordinates](../../../../../acceleration-in-polar-coordinates.md) is therefore zero:

$$
r\ddot\theta+2\dot r\dot\theta=0,
\qquad
\frac{d}{dt}(r^2\dot\theta)=0.
$$

Thus $\boxed{h=r^2\dot\theta\text{ is constant}}$; for unit mass it is the signed [angular momentum](../../../../../angular-momentum.md) perpendicular to the orbital plane. The radial component gives

$$
\ddot r-r\dot\theta^2=-\frac Q{r^2},\qquad
\ddot r=\frac{h^2}{r^3}-\frac Q{r^2}=-U'(r),
\qquad U(r)=\frac{h^2}{2r^2}-\frac Qr.
$$

Consequently

$$
\frac{d}{dt}\left(\frac12\dot r^2+U(r)\right)
=\dot r\bigl(\ddot r+U'(r)\bigr)=0,
\qquad
\boxed{E=\frac12\dot r^2+U(r)\text{ is constant}.}
$$

This is the [mechanical energy](../../../../../mechanical-energy.md), since the full [kinetic energy](../../../../../kinetic-energy.md) is $\tfrac12(\dot r^2+r^2\dot\theta^2)$ and $r^2\dot\theta^2=h^2/r^2$.

For $h\ne0$ and $Q>0$, the [effective potential](../../../../../effective-potential.md) goes to $+\infty$ as $r\downarrow0$ and to zero from below as $r\to\infty$. Its derivative is $U'(r)=(Qr-h^2)/r^3$, so it decreases up to $r_0=h^2/Q$ and then increases. Its zero and minimum are

$$
\boxed{U\left(\frac{h^2}{2Q}\right)=0,\qquad
r_0=\frac{h^2}{Q},\qquad U(r_0)=-\frac{Q^2}{2h^2}.}
$$

For $Q<0$, $U=h^2/(2r^2)+|Q|/r$ is positive and strictly decreasing, with limits $+\infty$ at zero and $0^+$ at infinity. It has no minimum at a finite positive radius.

<a id="10b/image-attractive-and-repulsive-inverse-square-effective-potentials-and-bounded-orbit-turning-points"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4-effective-potential.png)

**[Figure 2](#10b/image-attractive-and-repulsive-inverse-square-effective-potentials-and-bounded-orbit-turning-points). Attractive and repulsive inverse-square effective potentials and bounded-orbit turning points**.

If $h=0$, the centrifugal term disappears. For $Q>0$ the graph is instead $-Q/r$, increasing from $-\infty$ to $0^-$ without a minimum; for $Q<0$ it remains positive and decreasing. The bounded-orbit calculation below uses the stipulated $h>0$, which excludes this radial collision case.

## ↑ Ancestors (10)

1. [10B](../10b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
