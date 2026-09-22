<h1 id="section-d/d13/solution">Solution</h1>

↑ **Parent:** [D13](../d13.md)

[Snell's law](../../../../../snell-s-law.md) is $n_1\sin\theta_1=n_2\sin\theta_2$, with angles measured from the interface normal. The [Huygens-Fresnel principle](../../../../../huygens-fresnel-principle.md) explains it by constructing the transmitted [wavefront](../../../../../wavefront.md) from secondary wavelets: during the same time interval, distances travelled in the two media are proportional to $c/n_1$ and $c/n_2$. The geometry of the advancing plane [wavefront](../../../../../wavefront.md) then gives $\sin\theta_1/\sin\theta_2=(c/n_1)/(c/n_2)=n_2/n_1$.

For incidence from index $n$ into vacuum, the transmitted angle is $\alpha=\arcsin(n\sin\theta)$. The ray bends away from the normal, so its positive deviation is

$$
\boxed{\delta(\theta,n)=\arcsin(n\sin\theta)-\theta.}
$$

For $0<\theta<\theta_c=\arcsin(1/n)$,

$$
\frac{\partial\delta}{\partial\theta}=\frac{n\cos\theta}{\sqrt{1-n^2\sin^2\theta}}-1>0.
$$

Thus the graph rises monotonically from zero to a finite endpoint with a vertical tangent:

$$
\boxed{\theta_c=\arcsin(1/n),\qquad \delta_{\max}=\frac\pi2-\arcsin(1/n).}
$$

At the endpoint the transmitted ray grazes the interface. Beyond the [critical angle for total internal reflection](../../../../../critical-angle-for-total-internal-reflection.md), no propagating transmitted ray exists and [total internal reflection](../../../../../total-internal-reflection.md) occurs.

Inside a [prism](../../../../../prism-geometry.md), the two ray angles with the face normals sum to its apex angle. For the equilateral cross-section, they are $\theta$ and $\pi/3-\theta$. The entry deviation equals the corresponding exit deviation under ray reversal. Adding the two changes of direction therefore gives

$$
\boxed{\Delta(\theta)=\delta(\theta,n)+\delta(\pi/3-\theta,n).}
$$

This is symmetric about $\theta=\pi/6$. Symmetry alone gives a stationary point; to establish that it is a minimum, differentiate once more:

$$
\frac{\partial^2\delta}{\partial\theta^2}=\frac{n(n^2-1)\sin\theta}{(1-n^2\sin^2\theta)^{3/2}}>0
$$

within the transmitted-ray interval. The sum is therefore strictly convex, and

$$
\boxed{\theta_{\min}=\frac\pi6,\qquad \Delta_{\min}=2\arcsin(n/2)-\frac\pi3.}
$$

These expressions require $1<n<2$ for a non-grazing path through both faces; $n=2$ is a grazing limit, and $n>2$ admits no such two-face transmitted path. More explicitly, both internal angles must be at most $\theta_c$, which is possible only if $2\theta_c\geq\pi/3$.

<a id="section-d/d13/image-single-interface-deviation-and-the-symmetric-minimum-of-an-equilateral-prism-illustrated-for-index-1-5"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-prism-deviation.png)

**[Figure 6](#section-d/d13/image-single-interface-deviation-and-the-symmetric-minimum-of-an-equilateral-prism-illustrated-for-index-1-5). Single-interface deviation and the symmetric minimum of an equilateral prism, illustrated for index 1.5**.

Atmospheric hexagonal ice crystals can present pairs of faces with a $60^\circ$ angle, acting as small [prisms](../../../../../prism-geometry.md). Their orientations turn the minimum-deviation cone around the Moon into an [optical halo](../../../../../optical-halo.md). No transmitted ray of this family is deflected less than the [minimum deviation of a prism](../../../../../minimum-deviation-of-a-prism.md). Moreover, near the minimum, $\Delta-\Delta_{\min}$ is quadratic in the departure from the symmetric ray, so a range of incident directions is compressed into a small outgoing angular range. **This [caustic](../../../../../wave-caustic.md) makes the inner rim sharp and bright**, with the ray density decreasing farther outside. The common [22-degree halo](../../../../../22-degree-halo.md) has an angular radius near $22^\circ$ about either the Sun or Moon, hence a diameter near $44^\circ$.[Section 3.2.3.1.1: radius, central luminary, bright ring and darker interior](../../../../../international-cloud-atlas-by-world-meteorological-organization.md)

## ↑ Ancestors (13)

1. [D13](../d13.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
