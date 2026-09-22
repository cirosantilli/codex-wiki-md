<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

In the [Carnot cycle](../../../../../carnot-cycle.md), let $1\to2$ be reversible [isothermal expansion](../../../../../isothermal-expansion.md) at $T_h$, $2\to3$ reversible [adiabatic expansion](../../../../../adiabatic-expansion.md), $3\to4$ [isothermal compression](../../../../../isothermal-compression.md) at $T_c$, and $4\to1$ [adiabatic compression](../../../../../adiabatic-compression.md). The [pressure](../../../../../pressure-split.md)–[volume](../../../../../volume.md) curve is clockwise. The [entropy](../../../../../entropy-split.md)–[temperature](../../../../../temperature-split.md) figure below uses [temperature](../../../../../temperature-split.md) on the horizontal axis and [entropy](../../../../../entropy-split.md) on the vertical axis, literally an $S$–$T$ plot: isotherms are vertical and adiabats horizontal. The hot isotherm increases [entropy](../../../../../entropy-split.md) by $\Delta S$ and absorbs $Q_h=T_h\Delta S$; the cold one rejects $Q_c=T_c\Delta S$. Thus $W=(T_h-T_c)\Delta S$ and $\eta_C=1-T_c/T_h$.

For the second engine, choose the working direction with [heat](../../../../../heat-split.md) addition during $A\to B$ at $p_1$ and rejection during $C\to D$ at $p_2$. A [reversible ideal-gas adiabat](../../../../../reversible-ideal-gas-adiabat.md) obeys $T\propto p^{(\gamma-1)/\gamma}$. Define

$$
r=\left(\frac{p_1}{p_2}\right)^{(\gamma-1)/\gamma}>1,\qquad
\frac{T_B}{T_C}=\frac{T_A}{T_D}=r.
$$

The two constant-pressure [heat](../../../../../heat-split.md) transfers are $Q_{\rm in}=c_p(T_B-T_A)$ and $Q_{\rm out}=c_p(T_C-T_D)=Q_{\rm in}/r$, where rejected [heat](../../../../../heat-split.md) is quoted positive. Therefore the [Brayton cycle](../../../../../brayton-cycle.md) efficiency is

$$
\eta=1-\frac1r,\qquad
\boxed{\eta_{\rm mono}=1-\left(\frac{p_2}{p_1}\right)^{2/5}}
$$

for $\gamma=5/3$. All heat-capacity amount conventions cancel in the ratio.

Since $T_B>T_A$ and $T_C=T_B/r$, $T_D=T_A/r$, the maximum is **at B** and the minimum **at D**. The [Brayton-Carnot efficiency comparison](../../../../../brayton-carnot-efficiency-comparison.md) is

$$
\eta_C-\eta
=\left(1-\frac{T_D}{T_B}\right)-\left(1-\frac1r\right)
=\frac1r\left(1-\frac{T_A}{T_B}\right)>0.
$$

The inequality is strict for a nondegenerate cycle with positive [heat](../../../../../heat-split.md) input. Although each process can be reversible, the isobaric [heat](../../../../../heat-split.md) transfer spans a range of [temperatures](../../../../../temperature-split.md); making the whole cycle reversible requires a succession of matched-temperature reservoirs, rather than just the hottest and coldest reservoirs.

For an ideal diatomic gas with active rotation and frozen vibration, $\gamma=7/5$ and

$$
\eta_{\rm diatomic}=1-\left(\frac{p_2}{p_1}\right)^{2/7}<1-\left(\frac{p_2}{p_1}\right)^{2/5}.
$$

Here $0<p_2/p_1<1$. This comparison holds at the same [pressure](../../../../../pressure-split.md) ratio and assumes temperature-independent [heat capacities](../../../../../heat-capacity.md) in the stated mode regime. Frozen rotation or excited vibration would require their actual [heat capacities](../../../../../heat-capacity.md).

<a id="section-c/c12/image-carnot-and-brayton-cycles"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1-engine-cycles.png)

**[Figure 5](#section-c/c12/image-carnot-and-brayton-cycles). Carnot and Brayton cycles**.

## ↑ Ancestors (14)

1. [C12](../c12.md)
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
