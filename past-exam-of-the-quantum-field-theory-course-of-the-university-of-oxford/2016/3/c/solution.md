<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the notation $\Delta_{12}=\Delta(y_1-y_2)$, $\Delta_{xz}=\Delta(x-z)$ and $\int_{xz}=\int d^Dx\,d^Dz$. The order-$\lambda$ term vanishes because it has five [fields](../../../../field.md). At order $\lambda^2$, enumerate the eight-field [Wick contractions](../../../../wick-contraction.md), whose expansion denominator is $2!(3!)^2=72$.

If the two external [fields](../../../../field.md) contract with each other, the remaining [vacuum diagrams](../../../../vacuum-feynman-diagram.md) are a pair of cubic [vertices](../../../../vertex-graph-theory.md) joined by three lines, with six [Wick contractions](../../../../wick-contraction.md), and a pair joined by one line with a [tadpole diagram](../../../../tadpole-diagram.md) at each end, with nine [Wick contractions](../../../../wick-contraction.md). Define their combined integrated weight by

$$
V_2=\int_{xz}\left[\frac1{12}\Delta_{xz}^3+\frac18t^2\Delta_{xz}\right].
$$

Thus $Z/Z_0=1+(-i\lambda)^2V_2+O(\lambda^4)$. The numerator is

$$
\begin{aligned}
\frac{\mathcal N_2}{Z_0}
={}&\Delta_{12}\left[1+(-i\lambda)^2V_2\right]\quad+\\
&(-i\lambda)^2\int_{xz}\left[
\frac12K_1(x)K_2(z)\Delta_{xz}^2
+\frac12K_1(x)K_2(x)\Delta_{xz}t
+\frac14K_1(x)K_2(z)t^2\right]+O(\lambda^4).
\end{aligned}
$$

The three latter terms have respectively 36, 36 and 18 [Wick contractions](../../../../wick-contraction.md). Together with the six and nine [Wick contractions](../../../../wick-contraction.md), they exhaust all $7!!=105$ pairings.

Dividing by $Z/Z_0$ cancels the two [vacuum diagrams](../../../../vacuum-feynman-diagram.md), giving

$$
\boxed{\begin{aligned}
\langle T\phi(y_1)\phi(y_2)\rangle={}&\Delta_{12}+(-i\lambda)^2\int_{xz}\Bigl[
\tfrac12K_1(x)K_2(z)\Delta_{xz}^2\\
&+\tfrac12K_1(x)K_2(x)\Delta_{xz}t
+\tfrac14K_1(x)K_2(z)t^2\Bigr]+O(\lambda^4).
\end{aligned}}
$$

The first correction is the two-line [bubble diagram](../../../../bubble-diagram.md), with [symmetry factor](../../../../feynman-diagram-symmetry-factor.md) $S=2$. The second is the connected [tadpole contribution to a cubic-theory two-point function](../../../../tadpole-contribution-to-a-cubic-theory-two-point-function.md): both external lines meet one [vertex](../../../../vertex-graph-theory.md), joined by a single line to a second [vertex](../../../../vertex-graph-theory.md) bearing a [tadpole diagram](../../../../tadpole-diagram.md); its [symmetry factor](../../../../feynman-diagram-symmetry-factor.md) is also $S=2$. Interchanging the two integrated [vertices](../../../../vertex-graph-theory.md) is already included in the 36 contractions and gives no extra factor.

The final term is the [disconnected Feynman diagram](../../../../disconnected-feynman-diagram.md) consisting of two separate one-point [tadpole diagrams](../../../../tadpole-diagram.md), with coefficient $1/4$. It survives [cancellation of vacuum bubbles](../../../../cancellation-of-vacuum-bubbles.md), since each component touches an external point. Indeed it is precisely the leading $\langle\phi(y_1)\rangle\langle\phi(y_2)\rangle$. It would disappear from the connected [two-point correlation function](../../../../two-point-correlation-function.md), but the question defines the full [correlation function](../../../../correlation-function.md). No [normal ordering](../../../../normal-ordering.md) or [tadpole subtraction](../../../../tadpole-subtraction.md) of the interaction was specified. All terms are depicted in [solution](../b/solution.md), and all [spacetime](../../../../spacetime.md) integrals remain unevaluated.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../b/solution.md)
