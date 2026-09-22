<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Orient the contour so that the plus side is on the left; for a positively oriented simple closed contour this is its interior. If $\zeta(s)$ is a smooth arclength parametrization with $\zeta(0)=t$, define the [Cauchy principal value](../../../../../cauchy-principal-value.md) by deleting a symmetric interval $|s|<\eta$ and taking $\eta\downarrow0$. This pairs the two singular sides at equal local arclength.

Near $t$, write $f(\zeta)=f(t)+[f(\zeta)-f(t)]$. The second term divided by $\zeta-t$ is regular because $f$ is analytic there. For the constant term, indent the contour on either side of $t$ by a small semicircle. Its limiting contribution to the Cauchy integral is $\pm f(t)/2$, while the remaining contour tends to its principal value. This proves the [Sokhotski–Plemelj theorem](../../../../../sokhotski-plemelj-theorem.md):

$$
w_\pm(t)=\pm\frac12 f(t)+\frac1{2\pi i}
\operatorname{PV}\int_\Gamma\frac{f(\zeta)}{\zeta-t}\,d\zeta.
$$

In particular $w_+-w_-=f$ and $w_++w_-=g$ for the given integral equation.

Define $W=w$ inside and $W=-w$ outside. Its jump is $W_+-W_-=w_++w_-=g$, and it vanishes at infinity. Therefore

$$
W(z)=\frac1{2\pi i}\int_\Gamma\frac{g(t)}{t-z}\,dt.
$$

Indeed, the difference between the two sides has no jump, extends analytically across the smooth contour, and vanishes at infinity; [Liouville's theorem](../../../../../liouville-theorem.md) makes it zero. Applying the [Sokhotski–Plemelj theorem](../../../../../sokhotski-plemelj-theorem.md) again,

$$
f=W_++W_-=\boxed{\frac1{\pi i}
\operatorname{PV}\int_\Gamma\frac{g(t)}{t-z}\,dt}.
$$

Thus the normalized closed-contour singular integral operator is its own inverse.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
