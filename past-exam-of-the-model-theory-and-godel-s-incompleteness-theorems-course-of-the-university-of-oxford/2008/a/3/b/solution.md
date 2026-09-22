<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $T=S\cup\{\neg X\}$ and assume $S\vdash P_S(\ulcorner X\urcorner)\to X$. In $T$, contraposition against its extra axiom gives $\neg P_S(\ulcorner X\urcorner)$.

Classical logic proves $(\neg X\to X)\to X$. By the [derivability conditions](../../../../../hilbert-bernays-lob-derivability-conditions.md),

$$
S\vdash P_S(\ulcorner\neg X\to X\urcorner)\to P_S(\ulcorner X\urcorner).
$$

Compose this with the supplied formalized deduction implication from $P_T(\ulcorner X\urcorner)$ to its left-hand side. Then $T$ proves

$$
P_T(\ulcorner X\urcorner)\to P_S(\ulcorner X\urcorner),
$$

and therefore

$$
T\vdash\neg P_T(\ulcorner X\urcorner).
$$

The other supplied assumption says this is impossible if $T$ is [first-order consistent](../../../../../first-order-consistency.md). Thus $T$ is inconsistent. By the deduction theorem, inconsistency after adjoining $\neg X$ yields $S\vdash\neg\neg X$, hence

$$
\boxed{S\vdash X.}
$$

This establishes Löb's [inference rule](../../../../../inference-rule.md) using precisely the strengthened unprovability assumption and the formalized deduction property supplied in the question.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
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
