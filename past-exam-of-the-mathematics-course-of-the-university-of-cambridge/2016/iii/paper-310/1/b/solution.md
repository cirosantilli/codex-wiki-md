<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Insert the component-density laws into the [Friedmann equation](../../../../../../friedmann-equations.md), using $\rho_{i,0}=3H_0^2\Omega_{i,0}/(8\pi G)$ and $a_0=1$. Multiplying by $a^2$ gives

$$
\boxed{\dot a^2=H_0^2\left(\frac{\Omega_{r,0}}{a^2}
+\frac{\Omega_{m,0}}a+\Omega_{\Lambda,0}a^2\right)-K.}
$$

The [radiation in cosmology](../../../../../../radiation-in-cosmology.md) and [pressureless matter](../../../../../../pressureless-matter.md) contributions add; the printed first formula has lost the plus sign between them. In the [Friedmann acceleration equation](../../../../../../friedmann-acceleration-equation.md), $\rho+3P=2\rho_r+\rho_m-2\rho_\Lambda$, so

$$
\boxed{\ddot a=-H_0^2\left(\frac{\Omega_{r,0}}{a^3}
+\frac{\Omega_{m,0}}{2a^2}-\Omega_{\Lambda,0}a\right).}
$$

Evaluating the first equation today gives $K=H_0^2(\Omega_{r,0}+\Omega_{m,0}+\Omega_{\Lambda,0}-1)$.

Now remove [dark energy](../../../../../../dark-energy.md) and assume a positive [pressureless matter](../../../../../../pressureless-matter.md) or [radiation in cosmology](../../../../../../radiation-in-cosmology.md) density, starting on an expanding branch. Let $f(a)=H_0^2(\Omega_{r,0}/a^2+\Omega_{m,0}/a)$. It decreases from infinity to zero, and $\dot a^2=f(a)-K$, while $\ddot a<0$. This immediately distinguishes all three cases of [spatial curvature of an FLRW universe](../../../../../../spatial-curvature-of-an-flrw-universe.md).

- **Closed, $K>0$.** There is a unique maximum size $a_{\max}$ with $f(a_{\max})=K$. Expansion from a [Big Bang](../../../../../../big-bang.md) slows to $\dot a=0$ and then becomes contraction, ending in a [Big Crunch](../../../../../../big-crunch.md). The turning point is reached in finite time because $f(a)-K$ has a simple zero there. The acceleration remains negative at the maximum, so it is a recollapse rather than a static state.
- **Open, $K<0$.** The expanding solution never stops because $\dot a^2=f(a)+|K|>0$. It expands forever, eventually approaching a [curvature-dominated universe](../../../../../../curvature-dominated-universe.md) with $\dot a\to\sqrt{|K|}$ and $a(t)\sim\sqrt{|K|}\,t$. Locally its late-time behavior approaches the empty [Milne universe](../../../../../../milne-model.md).
- **Spatially flat, $K=0$.** Expansion also continues forever, but $\dot a\to0$ instead of approaching a nonzero constant. With [pressureless matter](../../../../../../pressureless-matter.md) present, the late-time solution has $a\propto t^{2/3}$, the [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md) behavior; a flat solution containing only [radiation in cosmology](../../../../../../radiation-in-cosmology.md) has $a\propto t^{1/2}$. With both components, an early [radiation domination](../../../../../../radiation-domination.md) era gives way to [matter domination](../../../../../../matter-domination.md).

The early small-$a$ solution has $a\propto t^{1/2}$ if [radiation in cosmology](../../../../../../radiation-in-cosmology.md) is present, and $a\propto t^{2/3}$ for [pressureless matter](../../../../../../pressureless-matter.md) alone. The figure isolates the effect of curvature in three matter-only examples, rather than comparing models with the same present density parameters.

<a id="1/b/image-matter-only-scale-factor-evolution-closed-recollapse-flat-power-law-expansion-and-open-expansion-tending-to-a-constant-speed"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-310-matter-expansion.png)

**[Figure 1](#1/b/image-matter-only-scale-factor-evolution-closed-recollapse-flat-power-law-expansion-and-open-expansion-tending-to-a-constant-speed). Matter-only scale-factor evolution: closed recollapse, flat power-law expansion, and open expansion tending to a constant speed.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
