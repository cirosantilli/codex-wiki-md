<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

A [Carnot cycle](../../../../../carnot-cycle.md) consists of two reversible isothermal branches joined by two reversible adiabatic branches. Let the hot isothermal expansion run from volume $V_a$ to $V_b$, and the cold isothermal compression from $V_c$ to $V_d$. For $n$ moles of an [ideal gas](../../../../../ideal-gas-split.md), their absorbed and rejected [heat](../../../../../heat-split.md) magnitudes are

$$
Q_h=nRT_1\ln(V_b/V_a),\qquad Q_c=nRT_2\ln(V_c/V_d).
$$

On a reversible ideal-gas adiabat, $TV^{\gamma-1}$ is constant. Applying this to the two joining branches gives $V_b/V_a=V_c/V_d$. Therefore

$$
\frac{Q_c}{Q_h}=\frac{T_2}{T_1},\qquad \boxed{\eta_C=\frac{Q_h-Q_c}{Q_h}=1-\frac{T_2}{T_1}.}
$$

The result is independent of the gas's heat-capacity ratio. This derivation presumes the usual constant-heat-capacity ideal-gas model; more generally the equal entropy changes on the two isotherms give the same heat ratio without that restriction.

To establish the upper bound, suppose an engine were more efficient between these same two reservoirs. Use its output [work](../../../../../work.md) to drive a reversed [Carnot cycle](../../../../../carnot-cycle.md), scaled so that the work magnitudes match. For fixed work $W$, the hypothetical engine would take $W/\eta$ from the hot bath, whereas the reversed [Carnot cycle](../../../../../carnot-cycle.md) would return $W/\eta_C>W/\eta$ to it. The combined device would transfer [heat](../../../../../heat-split.md) from the cold bath to the hot bath without any net external [work](../../../../../work.md). That contradicts the [Clausius statement of the second law](../../../../../clausius-statement-of-the-second-law.md). Hence **no such two-reservoir engine can exceed $1-T_2/T_1$**.

For the triangular cycle, call the three successive vertices $A,B,C$, and measure [energies](../../../../../energy-split.md) in units of $p_0V_0$. For one mole of a monatomic [ideal gas](../../../../../ideal-gas-split.md), $U=3pV/2$, and positive [work](../../../../../work.md) done by the gas is $W=\int p\,dV$. The net values on the three complete branches are

$$
\begin{array}{c|rrr}
\text{branch}&\Delta U/(p_0V_0)&W/(p_0V_0)&Q_{\rm net}/(p_0V_0)\\\hline
A\to B&3/2&0&3/2\\
B\to C&0&3/2&3/2\\
C\to A&-3/2&-1&-5/2
\end{array}
$$

Thus the net [work](../../../../../work.md) is **$W_{\rm cycle}=p_0V_0/2$**, equal to the triangle's enclosed area.

There is a small but important distinction between the net heat on a branch and its total positive [heat input to a cycle](../../../../../heat-input-to-a-cycle.md). On the sloping branch put $x=V/V_0$, so $p/p_0=3-x$, with $1\leq x\leq2$. Then

$$
\frac{U}{p_0V_0}=\frac32x(3-x),\qquad \frac{\delta Q}{p_0V_0}=\left(\frac{15}{2}-4x\right)dx.
$$

There is a [heat-flow reversal along a thermodynamic path](../../../../../heat-flow-reversal-along-a-thermodynamic-path.md) at $x=15/8$. The first part absorbs heat; the final part rejects it. Integrating the two signed contributions separately gives

$$
\frac{Q_{BC,+}}{p_0V_0}=\int_1^{15/8}\left(\frac{15}{2}-4x\right)dx=\frac{49}{32},\qquad \frac{Q_{BC,-}}{p_0V_0}=\int_{15/8}^2\left(\frac{15}{2}-4x\right)dx=-\frac1{32}.
$$

The true total absorbed and rejected [heats](../../../../../heat-split.md) and [thermal efficiency](../../../../../thermal-efficiency.md) are therefore

$$
\boxed{Q_{\rm in}=\frac{97}{32}p_0V_0,\qquad Q_{\rm out}=\frac{81}{32}p_0V_0,\qquad\eta=\frac{W_{\rm cycle}}{Q_{\rm in}}=\frac{16}{97}\simeq0.16495.}
$$

For clarity, the positive heat input on $A\to B$ is $3p_0V_0/2$, on $B\to C$ it is $49p_0V_0/32$, and on $C\to A$ it is zero. Using just the positive net heats of the complete branches would give $Q_{\rm in}=3p_0V_0$ and $\eta=1/6$; that shortcut misses the short heat-rejection interval on $B\to C$.

<a id="section-c/c10/image-original-pressure-volume-cycle-with-the-interior-temperature-maximum-and-the-late-reversal-of-heat-flow"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2-triangular-cycle.png)

**[Figure 3](#section-c/c10/image-original-pressure-volume-cycle-with-the-interior-temperature-maximum-and-the-late-reversal-of-heat-flow). Original pressure-volume cycle with the interior temperature maximum and the late reversal of heat flow**.

Finally, put $T_0=p_0V_0/R$. The minimum [temperature](../../../../../temperature-split.md) is $T_0$ at $A$. Along $B\to C$,

$$
T/T_0=x(3-x),
$$

which has its maximum $9/4$ at $x=3/2$, not at either endpoint. Thus the corresponding two-reservoir [Carnot efficiency](../../../../../carnot-efficiency.md) is

$$
\boxed{\eta_{C,\rm extremes}=1-\frac{T_{\min}}{T_{\max}}=1-\frac49=\frac59\simeq0.556.}
$$

The triangular cycle receives heat at a range of temperatures below $T_{\max}$ and rejects it at temperatures above $T_{\min}$. It therefore makes less [work](../../../../../work.md) per unit input [heat](../../../../../heat-split.md) than a [Carnot cycle](../../../../../carnot-cycle.md) using only those extrema. The geometric path alone does not prove irreversibility: it could in principle exchange heat reversibly with a continuum of matched-temperature reservoirs, while still having this lower efficiency. Restricting it to only the two extreme-temperature reservoirs would introduce additional irreversible heat transfers.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
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
