<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take a three-world [Kripke model for intuitionistic propositional logic](../../../../../../kripke-model-for-intuitionistic-propositional-logic.md) with a root $r$ and two incomparable terminal successors $u$ and $v$. Force $p$ only at $u$, force $q$ only at $v$, and force neither atom at $r$.

At $u$, the atom $p$ holds, so $u\Vdash\neg\neg p$, while $u\nVdash q$. Therefore

$$
r\nVdash\neg\neg p\to q.
$$

Likewise $v\Vdash\neg\neg q$ and $v\nVdash p$, so

$$
r\nVdash\neg\neg q\to p.
$$

The [Kripke forcing relation](../../../../../../kripke-forcing-relation.md) for a disjunction requires one disjunct to be forced at the current world. Consequently

$$
r\nVdash(\neg\neg p\to q)\vee(\neg\neg q\to p),
$$

which is the required [Kripke countermodel](../../../../../../kripke-countermodel.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
