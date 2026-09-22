<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The language of [Gödel-Löb logic](../../../../../godel-lob-logic.md) has [propositional variables](../../../../../propositional-variable.md), $\bot$, implication, and the unary operator $\Box$; the other [logical connectives](../../../../../logical-connective.md) are abbreviations. Its axioms are all classical [tautologies](../../../../../tautology.md), the distribution scheme $\Box(A\to B)\to(\Box A\to\Box B)$, and the Löb scheme $\Box(\Box A\to A)\to\Box A$. Its rules are [modus ponens rule](../../../../../implication-elimination-rule.md), [necessitation rule](../../../../../necessitation-rule.md) of theorems, and uniform substitution.

For a single boxed equation $p\leftrightarrow\Box C(p)$, set $F=\Box C(\top)$. The identity supplied in the source gives directly $GL\vdash F\leftrightarrow\Box C(F)$. If $p$ does not occur, take $F=\Box C$ instead.

Proceed by induction for a system of $m$ equations, allowing other [propositional variables](../../../../../propositional-variable.md) as parameters. Treat $p_1,\ldots,p_{m-1}$ as parameters in the last equation and put

$$
D(p_1,\ldots,p_{m-1})=\Box C_m(p_1,\ldots,p_{m-1},\top).
$$

The one-variable result proves $D\leftrightarrow\Box C_m(p_1,\ldots,p_{m-1},D)$. Substitute this $D$ for $p_m$ in the first $m-1$ equations. They are still boxed equations, so induction supplies solutions $F_1,\ldots,F_{m-1}$. Define $F_m=D(F_1,\ldots,F_{m-1})$.

By construction, the first $m-1$ equations hold after this substitution; substituting into the theorem for $D$ proves the last. Hence

$$
\boxed{GL\vdash F_i\leftrightarrow\Box C_i(F_1,\ldots,F_m)\quad(1\leq i\leq m).}
$$

The elimination introduces no new parameter letters and removes every unknown letter. This gives a constructive [simultaneous boxed fixed-point elimination in GL](../../../../../simultaneous-boxed-fixed-point-elimination-in-gl.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
