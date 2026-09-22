<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

Keep the problem's one-mole convention throughout. The excluded-volume parameter $b$ represents the loss of available translational [volume](../../../../../volume.md) due to short-range repulsion; it is an effective covolume, not simply the literal molecular material [volume](../../../../../volume.md). The attraction parameter $a$ reduces the [pressure](../../../../../pressure-split.md) below its purely repulsive value. In a mean-field picture, interaction [energy](../../../../../energy-split.md) is proportional to pair [density](../../../../../density.md), so the attractive free-energy contribution scales as $-a/V$ for one mole and the [pressure](../../../../../pressure-split.md) correction as $-a/V^2$. Equivalently, molecular cohesive [forces](../../../../../force-split.md) and the number striking a wall each supply a [density](../../../../../density.md) factor. These parameters approximate microscopic correlations rather than measuring every pair potential exactly.

At fixed [temperature](../../../../../temperature-split.md), $dF=-p\,dV$. Substituting $p=RT/(V-b)-a/V^2$ and integrating gives the [isothermal free-energy change of a Van der Waals gas](../../../../../isothermal-free-energy-change-of-a-van-der-waals-gas.md)

$$
\boxed{\Delta F=-RT\ln\frac{V_2-b}{V_1-b}+a\left(\frac1{V_1}-\frac1{V_2}\right).}
$$

The arbitrary temperature-only term cancels. The internal-energy [derivative](../../../../../derivative.md) is instead

$$
\left(\frac{\partial U}{\partial V}\right)_T
=T\left(\frac{\partial p}{\partial T}\right)_V-p=\frac a{V^2},\qquad
\boxed{\Delta U=a\left(\frac1{V_1}-\frac1{V_2}\right).}
$$

Expansion raises the attractive [internal energy](../../../../../internal-energy-split.md) toward zero. As a check, the [entropy](../../../../../entropy-split.md) change is $R\ln[(V_2-b)/(V_1-b)]$, so $\Delta F=\Delta U-T\Delta S$. Constant $a,b$ and a homogeneous branch with $V>b$ are assumed. If a subcritical equilibrium path crosses coexistence, a [Maxwell construction](../../../../../maxwell-construction.md) replaces the unstable homogeneous continuation; the displayed integral is the direct equation-of-state result, not a claim that such a continuation is physically stable.

At the [Van der Waals critical point](../../../../../van-der-waals-critical-point.md), the critical isotherm has a stationary inflection:

$$
0=-\frac{RT_c}{(V_c-b)^2}+\frac{2a}{V_c^3},\qquad
0=\frac{2RT_c}{(V_c-b)^3}-\frac{6a}{V_c^4}.
$$

Equating the resulting expressions for $RT_c$ gives $2V_c=3(V_c-b)$, hence

$$
V_c=3b,\qquad RT_c=\frac{8a}{27b},\qquad p_c=\frac{a}{27b^2},\qquad
\boxed{\frac{p_cV_c}{RT_c}=\frac38.}
$$

In reduced variables $x=V/V_c$, the critical curve is $p/p_c=8/(3x-1)-3/x^2$: it decreases through $(1,1)$ with zero first and second [derivative](../../../../../derivative.md), rather than having separate liquid/gas turning points at the critical [temperature](../../../../../temperature-split.md).

<a id="section-c/c11/image-critical-van-der-waals-isotherm"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1-critical-isotherm.png)

**[Figure 4](#section-c/c11/image-critical-van-der-waals-isotherm). Critical Van der Waals isotherm**.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
