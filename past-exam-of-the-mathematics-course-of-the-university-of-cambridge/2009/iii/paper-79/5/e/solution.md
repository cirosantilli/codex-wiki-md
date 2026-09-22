<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [hydraulic control of a zero-PV rotating channel](../../../../../../hydraulic-control-of-a-zero-pv-rotating-channel.md) is a critical section separating the upstream branch, where long-wave disturbances can propagate upstream, from the downstream branch, where they cannot. In the steady specific-energy description it is a stationary point of $E$ with respect to depth at fixed [volume flux](../../../../../../volumetric-flow-rate.md) and local width. The control therefore fixes the discharge for a given upstream [Bernoulli function](../../../../../../bernoulli-function.md) and channel geometry; an arbitrary downstream condition cannot generally be imposed independently on the upstream reservoir.

Evaluate all quantities at $x=0$ and keep $Q,b$ fixed while differentiating. With $\Delta=fb$, the preceding branch gives

$$
\frac{\partial u_1}{\partial h_1}=\frac g\Delta\left(1-\frac{h_1}{h_2}\right),\qquad \frac{\partial E}{\partial h_1}=1+\frac{u_1}{\Delta}\left(1-\frac{h_1}{h_2}\right).
$$

At the [hydraulic control of a zero-PV rotating channel](../../../../../../hydraulic-control-of-a-zero-pv-rotating-channel.md), this derivative vanishes. Using $h_1-h_2=\Delta v/g$ reduces it to $u_1v=gh_2$, where $v=u_1+\Delta/2$. Equivalently,

$$
v\left(v+\frac\Delta2\right)=gh_1,\qquad v_c=\sqrt{gh_1+\frac{\Delta^2}{16}}-\frac\Delta4.
$$

Combining this with $Q=b h_1v-b\Delta v^2/(2g)$ cancels the quadratic term and leaves

$$
\boxed{Q_c=\frac bg\left[\sqrt{gh_1+\frac{b^2f^2}{16}}-\frac{bf}{4}\right]^3.}
$$

At control $u_{1c}=\sqrt{gh_1+\Delta^2/16}-3\Delta/4$ and $h_{2c}=u_{1c}v_c/g$. Both walls must remain wet. Since $v_c>0$, the second depth is positive precisely when $u_{1c}>0$, giving

$$
\boxed{bf<\sqrt{2gh_1},\qquad b<\frac{\sqrt{2gh_1}}{f}.}
$$

Equality is the limiting case $u_{1c}=h_{2c}=0$, with the second wall just dry. For a wider channel, a dry lateral region requires a different solution and the two-wet-wall [hydraulic control of a zero-PV rotating channel](../../../../../../hydraulic-control-of-a-zero-pv-rotating-channel.md) formula cannot be continued. The channel must also remain sufficiently long and slowly varying for the transverse [geostrophic balance](../../../../../../geostrophic-balance.md) approximation to hold. As a check, $f\to0$ gives $Q_c=b\sqrt g\,h_1^{3/2}$, the familiar rectangular-channel critical discharge.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
