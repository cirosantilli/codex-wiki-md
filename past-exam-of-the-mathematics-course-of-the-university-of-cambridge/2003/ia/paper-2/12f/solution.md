<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

By rotational invariance, fix the first landing point at the north pole of a [sphere](../../../../../sphere.md) of radius $R$. A band of central angle $\theta$ and width $d\theta$ has area $2\pi R^2\sin\theta\,d\theta$. Dividing by total area gives the [central angle between independent uniform sphere points](../../../../../central-angle-between-independent-uniform-sphere-points.md) density

$$
\boxed{f_\Theta(\theta)=\tfrac12\sin\theta,\quad0<\theta<\pi,}
$$

and zero outside this range. The radius cancels.

Given the first pair's central angle $\gamma$, the third point can communicate with each of them exactly when it lies in that point's positive [hemisphere](../../../../../hemisphere.md). Choose their intersection line as a polar axis. Each [hemisphere](../../../../../hemisphere.md) permits an azimuth interval of length $\pi$, and the intervals' centres are separated by $\gamma$. Their overlap is a [spherical lune](../../../../../spherical-lune.md) of opening $\pi-\gamma$, with area $2R^2(\pi-\gamma)$. Therefore

$$
\mathbb P(C\text{ linked to both}\mid\gamma)=\frac{\pi-\gamma}{2\pi}.
$$

The union [probability](../../../../../probability.md) follows from inclusion-exclusion for two [hemispheres](../../../../../hemisphere.md):

$$
\mathbb P(C\text{ linked to at least one}\mid\gamma)
=\frac12+\frac12-\frac{\pi-\gamma}{2\pi}
=\frac12+\frac{\gamma}{2\pi}.
$$

Thus the requested conditional answers are

$$
\boxed{\mathbb P(C\text{ linked to either}\mid\gamma<\pi/2,\gamma)
=\frac12+\frac{\gamma}{2\pi},}
$$



$$
\boxed{\mathbb P(C\text{ linked to both}\mid\gamma>\pi/2,\gamma)
=\frac12-\frac{\gamma}{2\pi}.}
$$

“Either” here is inclusive: a third ship linked to both is also linked to at least one.

For network connectivity, if $\gamma<\pi/2$ the first pair is already linked, and the third must link to at least one of them. If $\gamma>\pi/2$, the first pair is not linked, and both must link through the third. Consequently the [connectivity of three acute-angle sphere points](../../../../../connectivity-of-three-acute-angle-sphere-points.md) is

$$
P_{\mathrm{conn}}=
\int_0^{\pi/2}\left(\frac12+\frac{\gamma}{2\pi}\right)\frac{\sin\gamma}{2}\,d\gamma
+\int_{\pi/2}^{\pi}\left(\frac12-\frac{\gamma}{2\pi}\right)\frac{\sin\gamma}{2}\,d\gamma.
$$

Using $\int_0^{\pi/2}\gamma\sin\gamma\,d\gamma=1$ and $\int_{\pi/2}^{\pi}\gamma\sin\gamma\,d\gamma=\pi-1$ gives

$$
\boxed{P_{\mathrm{conn}}=\frac12+\frac{2-\pi}{4\pi}=\frac{\pi+2}{4\pi}.}
$$

Angles exactly equal to the threshold have [probability](../../../../../probability.md) zero. Connectivity allows relaying and is weaker than requiring direct links between every pair.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
