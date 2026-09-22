<h1 id="section-c/c11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [diatomic molecule](../../../../../../diatomic-molecule.md) has one internal bond-stretching vibrational coordinate. Near its equilibrium separation, approximate the bond by a spring of stiffness $K$ and use the [reduced mass](../../../../../../reduced-mass.md) $\mu=m_1m_2/(m_1+m_2)$. Its [frequency](../../../../../../frequency.md) is $\omega=\sqrt{K/\mu}$ and its [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator-split.md) levels are $\epsilon_r=(r+1/2)\hbar\omega$.

For independent molecules in [thermal equilibrium](../../../../../../thermal-equilibrium-split.md), set $x=\hbar\omega/(k_BT)=\theta_v/T$. The single-molecule [canonical partition function](../../../../../../canonical-partition-function.md) is a [geometric series](../../../../../../geometric-series.md):

$$
z_v=\sum_{r=0}^\infty e^{-(r+1/2)x}=\frac{e^{-x/2}}{1-e^{-x}}.
$$

Using $U=-\partial\log(z_v^N)/\partial\beta$, where $\beta=1/(k_BT)$, gives

$$
U_v=N\hbar\omega\left(\frac12+\frac1{e^x-1}\right),\qquad \boxed{C_{V,v}=\left(\frac{\partial U_v}{\partial T}\right)_V=Nk_B\frac{x^2e^x}{(e^x-1)^2}.}
$$

Per mole replace $Nk_B$ by $R$. The [zero-point energy](../../../../../../zero-point-energy.md) is present in $U_v$ but is temperature-independent and contributes nothing to the [heat capacity](../../../../../../heat-capacity.md).

For $T\ll\theta_v$, occupation of the first excited vibrational state is exponentially suppressed: $C_{V,v}\simeq Nk_Bx^2e^{-x}\to0$. The vibrational degree of freedom is frozen out. For $T\gg\theta_v$, $C_{V,v}\to Nk_B$. This recovers classical equipartition: the quadratic kinetic term and quadratic elastic term each contribute $k_B/2$ per molecule.

<a id="section-c/c11/b/image-activation-of-a-diatomic-molecule-s-harmonic-vibrational-contribution-to-heat-capacity"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1-vibrational-heat-capacity.png)

**[Figure 4](#section-c/c11/b/image-activation-of-a-diatomic-molecule-s-harmonic-vibrational-contribution-to-heat-capacity). Activation of a diatomic molecule's harmonic vibrational contribution to heat capacity**.

The [vibrational heat capacity of a diatomic gas](../../../../../../vibrational-heat-capacity-of-a-diatomic-gas.md) must be distinguished from the total [heat capacity](../../../../../../heat-capacity.md). In a dilute gas with rotations already active and vibration still frozen, translation contributes $3R/2$ and rotation $R$, so molar $C_V\simeq5R/2$. Once vibration is active it adds $R$, giving $C_V\simeq7R/2$. For an ideal gas of a fixed number of intact molecules, $C_P=C_V+R$, so the corresponding values are $7R/2$ and $9R/2$. Very low temperatures also freeze rotations, while sufficiently high temperatures bring anharmonicity, dissociation or electronic excitations; the harmonic plateau is restricted to the range where those effects are negligible.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
