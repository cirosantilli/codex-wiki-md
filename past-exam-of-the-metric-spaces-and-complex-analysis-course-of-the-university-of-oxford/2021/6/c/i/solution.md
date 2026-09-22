<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

**There is no such map for the domain printed in the paper.** The planar [domain](../../../../../domain-mathematical-analysis.md) $A=\mathbb C\setminus[a,b]$ is not [simply connected](../../../../../simply-connected-space.md). For example, a sufficiently large positively oriented [circle](../../../../../circle.md) $\gamma$ surrounds $[a,b]$ and lies in $A$, while

$$
\int_\gamma\frac{dz}{z-a}=2\pi i\ne0.
$$

The integrand is [holomorphic](../../../../../holomorphic-function-split.md) on $A$. If $A$ were [simply connected](../../../../../simply-connected-space.md), the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) would force this [integral](../../../../../integral-split.md) to be zero. A [conformal bijection](../../../../../biholomorphism.md) is a [homeomorphism](../../../../../homeomorphism.md) and preserves [simple connectivity](../../../../../simply-connected-space.md), whereas $H$ is [simply connected](../../../../../simply-connected-space.md). Thus a [conformal bijection](../../../../../biholomorphism.md) $A\to H$ is impossible.

The explicit construction also pinpoints the missing point. Define

$$
T(z)=\frac{z-a}{z-b}.
$$

This [Möbius transformation](../../../../../mobius-transformation.md) sends the removed [line segment](../../../../../line-segment.md) to the nonpositive [real axis](../../../../../real-axis.md), together with infinity. More precisely, its [image](../../../../../image-of-a-function.md) on the stated planar [domain](../../../../../domain-mathematical-analysis.md) is

$$
T(A)=\bigl(\mathbb C\setminus(-\infty,0]\bigr)\setminus\{1\},
$$

since $T(z)=1$ has no finite solution when $a\ne b$. Conversely, its inverse $z=(bw-a)/(w-1)$ is defined for every $w$ in this set and cannot lie on $[a,b]$, proving this image description exactly.

Take the [principal square root](../../../../../principal-square-root-of-a-complex-number.md) of $T(z)$, characterized by positive [real part](../../../../../real-part.md), and then multiply by $i$. The result is the [conformal map](../../../../../conformal-map.md)

$$
\boxed{F(z)=i\sqrt{\frac{z-a}{z-b}}:\ A\longrightarrow H\setminus\{i\}.}
$$

Each stage is [injective](../../../../../injective-function.md) and onto the indicated [image](../../../../../image-of-a-function.md); the [square root](../../../../../square-root.md) maps the slit plane to the [right half-plane](../../../../../right-half-plane.md), with the point $1$ omitted here. Hence this is a [conformal bijection](../../../../../biholomorphism.md) onto the punctured [upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Its inverse is

$$
z=\frac{a+bF^2}{1+F^2}.
$$

If the source is instead $(\mathbb C\cup\{\infty\})\setminus[a,b]$ on the [Riemann sphere](../../../../../riemann-sphere.md), the same map extends with $F(\infty)=i$ and becomes a [conformal bijection](../../../../../biholomorphism.md) onto all of $H$. Indeed, in the local coordinate $u=1/z$ it has expansion $F=i+\tfrac i2(b-a)u+O(u^2)$, whose [derivative](../../../../../derivative.md) at $u=0$ is nonzero. This gives the sphere version of the requested construction without silently changing the printed planar [domain](../../../../../domain-mathematical-analysis.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [c](../../c.md)
3. [6](../../../6.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
