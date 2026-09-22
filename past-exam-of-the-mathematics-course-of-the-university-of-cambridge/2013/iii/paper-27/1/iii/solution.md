<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**As printed, the lower bound needs a connectedness hypothesis.** This illustrates that [radius gives no positive lower bound for disconnected harmonic hull capacity](../../../../../../radius-gives-no-positive-lower-bound-for-disconnected-harmonic-hull-capacity.md). A [compact H-hull](../../../../../../compact-h-hull.md) need not have connected closure. To see the obstruction, take $0<\varepsilon<1/12$, set $c=\sqrt{1-\varepsilon^2}$, and use three disjoint vertical slits,

$$
K_\varepsilon=(0,i\varepsilon]\cup(c,c+i\varepsilon]
\cup(-c,-c+i\varepsilon].
$$

Their complement in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) is a [simply connected domain](../../../../../../simply-connected-domain.md): the three slits attach to the real boundary, and create no interior holes. Symmetry shows that the smallest enclosing half-disc is centred at zero and has radius one. More explicitly, any real centre $b$ has maximum distance to the two outer tips at least $\sqrt{c^2+\varepsilon^2}=1$, while the unit half-disc contains every slit. Also $0\in\overline K_\varepsilon$ and $c+i\varepsilon$ has modulus one.

For a vertical slit of height $\varepsilon$, the [mapping-out function of a vertical slit](../../../../../../mapping-out-function-of-a-vertical-slit.md) maps its two faces onto an interval of length $2\varepsilon$, so its [harmonic capacity from infinity in the upper half-plane](../../../../../../harmonic-capacity-from-infinity-in-the-upper-half-plane.md) is $2\varepsilon$. [Subadditivity of harmonic hull capacity](../../../../../../subadditivity-of-harmonic-hull-capacity.md), from the union bound for the Brownian hitting events, gives

$$
\boxed{\operatorname{cap}(K_\varepsilon)\le6\varepsilon<\frac12.}
$$

Thus the requested conclusion does not follow from the printed assumptions.

The intended [reflection lower bound for harmonic hull capacity](../../../../../../reflection-lower-bound-for-harmonic-hull-capacity.md) works when the closure is a connected continuum joining the two specified points, as for a slit hull. Reflect in the vertical line through $x$, using $\rho(z)=2x-\bar z$. The reflected continuum joins $2x$ to $x+iy$. Together the original and reflected continua form a barrier between infinity and the segment $I$ together with the real interval between $0$ and $2x$. One can first verify this separation for polygonal simple arcs, then use decreasing connected neighbourhoods of the continuum. Hence, for Brownian motion started at $x+iY$, $Y$ large, reaching $I$ or the real interval $J$ between $0$ and $x$ requires a hit of the original or reflected barrier. Reflection symmetry and the union bound give

$$
\mathbb P_{x+iY}\bigl(B_{T(\mathbb H\setminus I)}\in I\cup J\bigr)
\le2\,\mathbb P_{x+iY}(B_{T(H)}\in\overline K).
$$

For the connected slit setting, the real attachment endpoints have zero [harmonic measure](../../../../../../harmonic-measure.md), so the last event may be written with $K$.

For $y>0$, use the branch of the square root fixed by [hydrodynamic normalization at infinity](../../../../../../hydrodynamic-normalization-at-infinity.md):

$$
g_I(z)=x+\sqrt{(z-x)^2+y^2}.
$$

The two slit faces together have image length $2y$. The interval $J$ has image length $\sqrt{x^2+y^2}-y=1-y$, by the square-root formula on the appropriate real side. Thus the image length of $I\cup J$ is $1+y$. Multiply the probability inequality by $\pi Y$ and use part (i); the allowed starting approach includes $x+iY$. We obtain

$$
\boxed{\operatorname{cap}(K)\ge\frac{1+y}{2}\ge\frac12}
$$

under the stated connected-barrier interpretation. If $y=0$, the model slit is empty and $J$ has length $|x|=1$, giving the same lower bound by the real-interval argument. The connectedness repair is essential, as the explicit three-slit counterexample demonstrates.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
