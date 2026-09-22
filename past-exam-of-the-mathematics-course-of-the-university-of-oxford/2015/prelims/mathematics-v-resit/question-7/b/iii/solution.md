<h1 id="question-7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use source [spherical coordinates](../../../../../../../spherical-coordinate-system.md) with radius $s$, polar angle $\alpha$ measured from the positive $z$-axis, and azimuth $\theta$. The lower half of the [spherical shell](../../../../../../../spherical-shell.md) has $a\leq s\leq2a$, $\pi/2\leq\alpha\leq\pi$, and $0\leq\theta\leq2\pi$. Its [volume element](../../../../../../../volume-element.md) is $s^2\sin\alpha\,ds\,d\alpha\,d\theta$. At the observation point $(0,0,h)$, $h>0$, the separation is $\sqrt{s^2+h^2-2sh\cos\alpha}$, so

$$
\phi(h)=-2\pi G\rho\int_a^{2a}s^2
\int_{\pi/2}^{\pi}\frac{\sin\alpha\,d\alpha}
{\sqrt{s^2+h^2-2sh\cos\alpha}}\,ds.
$$

The angular [integral](../../../../../../../integral-split.md) is elementary: put $q=\cos\alpha$ to obtain

$$
\int_{-1}^0\frac{dq}{\sqrt{s^2+h^2-2shq}}
=\frac{s+h-\sqrt{s^2+h^2}}{sh}.
$$

We used $\sqrt{(s+h)^2}=s+h$ since both $s,h$ are positive. Hence

$$
\begin{aligned}
\phi(h)
&=-\frac{2\pi G\rho}{h}\int_a^{2a}
\bigl(s^2+hs-s\sqrt{s^2+h^2}\bigr)\,ds\\
&=-\frac{2\pi G\rho}{h}
\left[\frac{s^3}{3}+\frac{hs^2}{2}
-\frac{(s^2+h^2)^{3/2}}{3}\right]_a^{2a}.
\end{aligned}
$$

Thus the [axial potential of a uniform hemispherical shell](../../../../../../../axial-potential-of-a-uniform-hemispherical-shell.md), at every point of the positive $z$-axis, is

$$
\boxed{\phi(h)=-\frac{2\pi G\rho}{3h}
\left[7a^3+\frac92ha^2-(4a^2+h^2)^{3/2}+(a^2+h^2)^{3/2}\right],\qquad h>0.}
$$

There is no need to split into $h<a$, $a<h<2a$, and $h>2a$: the observation point is outside the lower [hemisphere](../../../../../../../hemisphere.md) in all three cases. As checks, $\phi(h)\to-3\pi G\rho a^2$ as $h\downarrow0$, and at large $h$,

$$
\phi(h)\sim-\frac{G}{h}\,\frac{14\pi\rho a^3}{3}.
$$

The last factor is exactly the total [mass](../../../../../../../mass.md) of the lower half of the [spherical shell](../../../../../../../spherical-shell.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [Question 7](../../../question-7.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
