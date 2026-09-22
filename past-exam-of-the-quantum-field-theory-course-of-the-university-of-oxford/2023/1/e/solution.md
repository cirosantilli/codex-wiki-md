<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The additional six-leg [interaction vertex](../../../../interaction-vertex.md) has [Feynman rule](../../../../feynman-rule.md) $-ig_6$. Since both interactions lack derivatives, the graph identity still gives $\omega=2(1-V)$, with $V=V_4+V_6$. The difference is that a one-vertex contraction of the [phi-six theory](../../../../phi-six-theory.md) can leave four external legs: choosing the contracted pair gives $\binom62=15$. Its [quartic interaction](../../../../quartic-interaction.md) correction is

$$
\frac{g_6}{6!}\,15T_\Lambda\phi^4
=\frac1{4!}\frac{g_6T_\Lambda}{2}\phi^4.
$$

Consequently a one-loop [quartic interaction](../../../../quartic-interaction.md) [counterterm](../../../../counterterm.md) is now necessary:

$$
\boxed{\delta g_4^{(1)}=-\frac{g_6}{2}T_\Lambda
=-\frac{g_6}{8\pi}\log\left(1+\frac{\Lambda^2}{m^2}\right).}
$$

The one-loop [mass counterterm](../../../../mass-counterterm.md) from [c](../c.md) is unchanged. Contracting four legs of a single six-leg [interaction vertex](../../../../interaction-vertex.md) gives $\binom62\,3=45$ double contractions, hence a two-loop raw [self-energy](../../../../self-energy.md) $g_6T_\Lambda^2/8$. Its subtraction must include the [quartic interaction](../../../../quartic-interaction.md) [counterterm](../../../../counterterm.md) insertion, rather than subtracting this raw expression in isolation.

All divergent field-dependent coefficients are most simply organized by the [normal-ordering subtraction scheme in two dimensions](../../../../normal-ordering-subtraction-scheme-in-two-dimensions.md). With $T=T_\Lambda$, express a potential normal ordered at mass $m$ in ordinary fields:

$$
V_B(\phi)=\frac{g_4}{24}(\phi^4-6T\phi^2+3T^2)
+\frac{g_6}{720}(\phi^6-15T\phi^4+45T^2\phi^2-15T^3).
$$

Thus its divergent subtraction coefficients, in this scheme, are

$$
\boxed{\delta g_4=-\frac{g_6T}{2},\qquad
\delta_m=-\frac{g_4T}{2}+\frac{g_6T^2}{8},\qquad
\delta g_6=\delta_Z=0.}
$$

Indeed the two-loop [self-energy](../../../../self-energy.md) terms are $g_6T^2/8+\delta g_4T/2=-g_6T^2/8$, which the displayed [mass counterterm](../../../../mass-counterterm.md) cancels. The constant terms only affect [vacuum energy](../../../../vacuum-energy.md). After removing all one-vertex self-contractions, every remaining subgraph is [ultraviolet finite](../../../../ultraviolet-finiteness.md). Additional finite [on-shell renormalization scheme](../../../../on-shell-renormalization-scheme.md) adjustments are subject to the same qualification as [d](../d.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
