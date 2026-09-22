<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Fix deterministic $0\leq s<t$ and $A\in\mathcal F_s$. The [pasting ordered stopping times](../../../../../../pasting-ordered-stopping-times.md) argument shows that $U=s\mathbf1_A+t\mathbf1_{A^c}$ is a [bounded stopping time](../../../../../../bounded-stopping-time.md). The given stopped-expectation property, applied to $U$ and to the deterministic [stopping time](../../../../../../stopping-time.md) $t$, yields

$$
0=\mathbb E X_U-\mathbb E X_t=\mathbb E[(X_s-X_t)\mathbf1_A].
$$

This holds for every $A\in\mathcal F_s$. Since $X_s$ is $\mathcal F_s$-[measurable](../../../../../../measurability.md) and both time values are integrable, it is exactly the defining test for [conditional expectation](../../../../../../conditional-expectation.md):

$$
\boxed{\mathbb E[X_t\mid\mathcal F_s]=X_s.}
$$

Hence **$X$ is a [martingale](../../../../../../martingale-split.md)**. This proof of the [characterization of a martingale by bounded continuous-time stopped expectations](../../../../../../characterization-of-a-martingale-by-bounded-continuous-time-stopped-expectations.md) uses only deterministic two-time pastings; the [càdlàg](../../../../../../cadlag.md) assumption and the [usual conditions for a filtration](../../../../../../usual-conditions-for-a-filtration.md) are stronger than needed for this implication.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
