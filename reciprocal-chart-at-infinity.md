# Reciprocal chart at infinity

↑ **Parent:** [Holomorphic stereographic atlas of the sphere](holomorphic-stereographic-atlas-of-the-sphere.md)

The reciprocal chart makes infinity an ordinary coordinate origin. Its domain is the [Riemann sphere](riemann-sphere.md) minus the point $z=0$; $w(\infty)=0$ and $w(z)=1/z$ elsewhere. A [neighbourhood](neighbourhood-mathematics.md) $U_R$ of infinity becomes the [open disc](open-disc.md) $|w|<1/R$. In sphere coordinates this is exactly the cap

$$
Z>\frac{R^2-1}{R^2+1}.
$$

For $R=2$, the exterior $|z|>2$ together with infinity becomes $Z>3/5$ and $|w|<1/2$. The boundary itself is excluded from each [open set](open-set.md).

<a id="image-the-same-neighbourhood-of-infinity-as-a-plane-exterior-a-north-pole-cap-and-a-disc-in-the-reciprocal-chart"></a>
![](riemann-sphere-reciprocal-cap.png)

**[Figure 4](#image-the-same-neighbourhood-of-infinity-as-a-plane-exterior-a-north-pole-cap-and-a-disc-in-the-reciprocal-chart). The same neighbourhood of infinity as a plane exterior, a north-pole cap, and a disc in the reciprocal chart**.

The point $z=2+i$ lies in this [neighbourhood](neighbourhood-mathematics.md) because $|z|=\sqrt5>2$. Its reciprocal coordinate is $w=(2-i)/5$, with $|w|=1/\sqrt5<1/2$, and its sphere height is $Z=2/3>3/5$. The negative [imaginary part](imaginary-part.md) of $w$ is the axis reversal required by the [holomorphic stereographic atlas of the sphere](holomorphic-stereographic-atlas-of-the-sphere.md).

For a complex-valued [holomorphic function](holomorphic-function-split.md) $f$ defined outside a large disc, having a [removable singularity at infinity](removable-singularity-at-infinity.md) means that $g(w)=f(1/w)$ extends to a [holomorphic function](holomorphic-function-split.md) at $w=0$. This definition reduces questions at infinity to familiar questions at a finite point.[Complex Analysis Lecture Notes, section 9, items 81–82, printed p. 32, reciprocal definition at infinity](complex-analysis-lecture-notes-by-dan-romik.md) For example,

$$
f(z)=\frac{z-2}{z+3},\qquad g(w)=\frac{1-2w}{1+3w}=1-5w+15w^2-45w^3+\cdots,\qquad |w|<1/3.
$$

The [geometric series](geometric-series.md) gives a [Taylor series](taylor-series.md) at the new origin, so $f(\infty)=1$ and $g'(0)=-5$. The coefficient $-5$ is the [derivative](derivative.md) in the specified $w$ coordinate. In contrast, $f(z)=z^2$ becomes $g(w)=w^{-2}$, displaying a [pole](pole.md) of order two at infinity when the target is the [complex plane](complex-plane.md). As a [holomorphic map](holomorphic-map.md) to the [Riemann sphere](riemann-sphere.md), it uses the target reciprocal coordinate $1/f(1/w)=w^2$, which is regular at zero.

## ↑ Ancestors (9)

1. [Holomorphic stereographic atlas of the sphere](holomorphic-stereographic-atlas-of-the-sphere.md)
2. [Stereographic projection](stereographic-projection.md)
3. [Riemann sphere](riemann-sphere.md)
4. [Riemann surfaces](riemann-surfaces-split.md)
5. [Complex analysis](complex-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Riemann sphere](riemann-sphere.md)
