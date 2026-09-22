<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

**The [Second law of thermodynamics](../../../../../second-law-of-thermodynamics-split.md) restricts which energy-conserving processes can occur.** In the [Kelvin-Planck statement of the second law](../../../../../kelvin-planck-statement-of-the-second-law.md), no cyclic engine can have as its sole effect the extraction of [heat](../../../../../heat-split.md) from one reservoir and its complete conversion into work. In the [Clausius statement of the second law](../../../../../clausius-statement-of-the-second-law.md), no process can have as its sole effect transferring [heat](../../../../../heat-split.md) from a colder reservoir to a hotter one. An engine or refrigerator combined with the reverse of a reversible device shows that a violation of either statement would violate the other.

A [heat engine](../../../../../heat-engine.md) takes [heat](../../../../../heat-split.md) $Q_h>0$ from a reservoir at $T_h$, rejects $Q_c>0$ to one at $T_c<T_h$, and returns its working substance to the initial state. Energy conservation gives $W=Q_h-Q_c$ and efficiency $\eta=W/Q_h=1-Q_c/Q_h$. **[Carnot's theorem](../../../../../carnot-s-theorem.md)** states that no engine between these reservoirs is more efficient than a reversible one, and that all reversible engines between them have the same efficiency. Otherwise, drive a reversible engine backwards with the work of a more efficient engine; the composite cycle transfers [heat](../../../../../heat-split.md) from cold to hot without external work, contradicting the Clausius statement.

A reversible [Carnot cycle](../../../../../carnot-cycle.md) consists of two isotherms joined by two reversible adiabats. For an ideal gas, $Q_h=Nk_BT_h\log(V_2/V_1)$ and $Q_c=Nk_BT_c\log(V_3/V_4)$. The adiabats give $V_2/V_1=V_3/V_4$, so

$$
\boxed{\frac{Q_c}{Q_h}=\frac{T_c}{T_h},\qquad\eta_{\rm reversible}=1-\frac{T_c}{T_h}.}
$$

[Carnot's theorem](../../../../../carnot-s-theorem.md) makes this independent of the working substance and defines the thermodynamic absolute-[temperature](../../../../../temperature-split.md) scale consistently with ideal-gas [temperature](../../../../../temperature-split.md).[Sections 4.3.1–4.3.2: heat engines, Carnot's theorem and temperature](../../../../../classical-thermodynamics-by-david-tong.md)

For any reversible cycle, $\oint\delta Q_{\rm rev}/T=0$. This makes the integral between two equilibrium states independent of the reversible path, defining the [state function](../../../../../state-function.md) [entropy](../../../../../entropy-split.md):

$$
\boxed{S_B-S_A=\int_A^B\frac{\delta Q_{\rm rev}}T.}
$$

[Heat](../../../../../heat-split.md) itself is path dependent; [entropy](../../../../../entropy-split.md) is not. An irreversible change can be evaluated using any imagined reversible path between its equilibrium endpoints. For example, a fixed amount of ideal gas with constant $C_V$ has $\Delta S=C_V\log(T_B/T_A)+Nk_B\log(V_B/V_A)$.

For a general cycle the [Clausius inequality](../../../../../clausius-inequality.md) is $\oint\delta Q/T_{\rm boundary}\leq0$. The [entropy](../../../../../entropy-split.md) balance for a process is $\Delta S\geq\int\delta Q/T_{\rm boundary}$, with equality for reversible [heat](../../../../../heat-split.md) exchange and no [entropy production](../../../../../entropy-production.md). The surroundings' [entropy](../../../../../entropy-split.md) must be included, giving **$\Delta S_{\rm universe}\geq0$**. A system's own [entropy](../../../../../entropy-split.md) can decrease by exporting [entropy](../../../../../entropy-split.md); an isolated system's cannot.

The engine's reservoirs have net [entropy](../../../../../entropy-split.md) change $Q_c/T_c-Q_h/T_h\geq0$, so

$$
\boxed{\eta\leq1-\frac{T_c}{T_h},}
$$

with equality for a reversible engine. Friction, [heat](../../../../../heat-split.md) flow through a finite [temperature](../../../../../temperature-split.md) difference and unrestrained expansion produce [entropy](../../../../../entropy-split.md) and reduce usable work. Thus energy conservation fixes the balance of [heat](../../../../../heat-split.md) and work, while the second law fixes their direction and the attainable efficiency.[Section 4.3.3: entropy as a state function and the second law](../../../../../classical-thermodynamics-by-david-tong.md)

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
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
