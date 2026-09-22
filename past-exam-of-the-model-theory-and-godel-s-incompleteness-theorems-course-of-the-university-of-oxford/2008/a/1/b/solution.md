<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The definition of $a$ makes the diagonal instance $E_a[\bar a]$ exactly $G_S$. The representing [logical formula](../../../../../logical-formula.md) therefore has the standard interpretation

$$
\mathbb N\models\exists v_2A(\bar a,v_2)\quad\Longleftrightarrow\quad S\vdash G_S.
$$

If $S\vdash G_S$, choose an actual witness $m$ to the left-hand existential statement. The [bounded arithmetic sentence](../../../../../bounded-arithmetic-sentence.md) $A(\bar a,\bar m)$ is true and hence provable by $\Sigma_0$-completeness. But $G_S$ also gives $S\vdash\neg A(\bar a,\bar m)$, a [contradiction](../../../../../contradiction.md). Thus

$$
\boxed{S\text{ consistent}\quad\Longrightarrow\quad S\nvdash G_S.}
$$

Now assume [one-consistency](../../../../../one-consistency.md). It implies [first-order consistency](../../../../../first-order-consistency.md), so no [formal proof](../../../../../formal-proof.md) of $G_S$ exists and $A(a,m)$ is false for each standard $m$. Each [bounded arithmetic sentence](../../../../../bounded-arithmetic-sentence.md) $\neg A(\bar a,\bar m)$ is consequently true and provable. A [formal proof](../../../../../formal-proof.md) of $\neg G_S$ would give a [formal proof](../../../../../formal-proof.md) of $\exists v_2A(\bar a,v_2)$ while every standard witness instance is refuted, contrary to [one-consistency](../../../../../one-consistency.md). Hence

$$
\boxed{S\text{ one-consistent}\quad\Longrightarrow\quad S\nvdash\neg G_S.}
$$

The two hypotheses play different roles: ordinary [first-order consistency](../../../../../first-order-consistency.md) excludes the positive [Gödel sentence](../../../../../godel-sentence.md), while the stronger hypothesis also excludes its [negation](../../../../../negation.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
