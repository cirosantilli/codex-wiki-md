<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [Monge-gauge Hamiltonian of a three-dimensional string](../../../../../../monge-gauge-hamiltonian-of-a-three-dimensional-string.md), in [Monge gauge](../../../../../../monge-gauge.md), $X'^m=(0,1,\Phi')$ and $P_m=(P_0,P_1,\Pi)$. The [momentum](../../../../../../momentum.md) [constraint](../../../../../../constraint-mechanics.md) gives $P_1=-\Phi'\Pi$. The other [Virasoro constraint](../../../../../../virasoro-constraint.md) then reads

$$
-P_0^2+(\Phi'\Pi)^2+\Pi^2+1+\Phi'^2=0.
$$

Choosing the positive-energy branch,

$$
\boxed{P_1=-\Phi'\Pi,\qquad P_0=-\sqrt{(1+\Phi'^2)(1+\Pi^2)}.}
$$

Substituting into the [phase-space action](../../../../../../phase-space-action.md) leaves $I=\int dt\,d\sigma(\Pi\dot\Phi-\mathcal H)$, so

$$
\boxed{F(z)=1+z^2,\qquad \mathcal H=\sqrt{(1+\Phi'^2)(1+\Pi^2)},\qquad H=\int d\sigma\,\mathcal H.}
$$

For an infinite string this is an energy-density expression; even the undeformed string has infinite total [energy](../../../../../../energy.md). One may regulate the length or subtract its constant reference [energy](../../../../../../energy.md) when a finite total [energy](../../../../../../energy.md) is needed. The positive branch is unambiguous at the density level.

The canonical [Hamiltonian field equations](../../../../../../hamiltonian-field-equation.md) are

$$
\dot\Phi=\Pi\sqrt{\frac{1+\Phi'^2}{1+\Pi^2}},\qquad
\dot\Pi=\partial_\sigma\left(\Phi'\sqrt{\frac{1+\Pi^2}{1+\Phi'^2}}\right).
$$

Consequently $\Pi=\Phi'$ implies

$$
\boxed{\dot\Phi=\Phi',\qquad\Phi=f(\sigma+t).}
$$

The second equation also becomes $\dot\Pi=\Phi''$, consistent with differentiating the first. These are one-direction traveling profiles along the string.

For the linear profile, the spatial string is the straight line $X^2=kX^1+kt$. It is tilted, and its coordinate intercept moves with speed $k$. This is also a uniformly moving straight string: the [physical transverse velocity of a tilted string](../../../../../../physical-transverse-velocity-of-a-tilted-string.md) is the velocity normal to the line. With unit tangent $(1,k)/\sqrt{1+k^2}$ and coordinate velocity $(0,k)$, the normal speed is

$$
\boxed{v_\perp=\frac{|k|}{\sqrt{1+k^2}}<1.}
$$

Thus **$k>1$ does not imply superluminal physical motion**. Fixed-$\sigma$ labels have spacelike trajectories when $k>1$, but labels on a string can slide tangentially and are not identifiable material particles. Choosing $\dot\sigma=-k^2/(1+k^2)$ removes the tangential velocity and gives the subluminal velocity $(-k^2,k)/(1+k^2)$.

The [induced worldsheet metric](../../../../../../induced-worldsheet-metric.md) supplies a coordinate-invariant check:

$$
h_{tt}=k^2-1,\qquad h_{t\sigma}=k^2,\qquad h_{\sigma\sigma}=1+k^2,\qquad\boxed{\det h=-1.}
$$

The [string worldsheet](../../../../../../worldsheet.md) remains Lorentzian for every finite $k$, including $k=1$ and $k>1$. Its constant [energy density](../../../../../../energy-density.md) is $1+k^2$. This linear profile is a tilted boosted straight string, rather than a localized finite-energy wave.

<a id="2/ii/image-for-slope-k-2-the-vertical-coordinate-velocity-exceeds-one-while-its-component-normal-to-the-tilted-string-has-physical-speed-2-divided-by-the-square-root-of-5"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-306-transverse-motion.png)

**[Figure 1](#2/ii/image-for-slope-k-2-the-vertical-coordinate-velocity-exceeds-one-while-its-component-normal-to-the-tilted-string-has-physical-speed-2-divided-by-the-square-root-of-5). For slope k=2 the vertical coordinate velocity exceeds one, while its component normal to the tilted string has physical speed 2 divided by the square root of 5**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
