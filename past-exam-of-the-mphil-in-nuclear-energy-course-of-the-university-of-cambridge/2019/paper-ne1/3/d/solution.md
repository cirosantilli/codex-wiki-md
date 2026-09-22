<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Differentiate the family of steady states, keeping $T_i$, $W_C$, $c_C$, $R_1$ and $R_2$ fixed.** A [quasistatic process](../../../../../quasistatic-process.md) uses the temperature responses from part (b):

$$
\frac{d\overline T_C}{dP}=\frac1{2W_Cc_C},
\quad
\frac{d\overline T_M}{dP}=R_2+\frac1{2W_Cc_C},
\quad
\frac{d\overline T_F}{dP}=R_1+R_2+\frac1{2W_Cc_C}.
$$

Apply the [chain rule](../../../../../chain-rule.md) to [reactor reactivity](../../../../../reactivity-nuclear-engineering.md) along that family, weighting each response by its [temperature coefficient of reactivity](../../../../../temperature-coefficient-of-reactivity.md). Collecting terms gives the [power coefficient of reactivity](../../../../../power-coefficient-of-reactivity.md)

$$
\boxed{
\alpha_P
=\alpha_FR_1+(\alpha_F+\alpha_M)R_2
+\frac{\alpha_F+\alpha_M+\alpha_C}{2W_Cc_C}.
}
$$

Its unit is inverse [power](../../../../../power.md). If the [thermal resistances](../../../../../thermal-resistance.md), coolant flow or inlet condition varied appreciably with [power](../../../../../power.md), their derivatives would contribute additional terms; those changes are excluded by the stipulated constant-parameter model.

## ↑ Ancestors (10)

1. [D](../d.md)
2. [3](../../3.md)
3. [Module NE1](../../../paper-ne1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
