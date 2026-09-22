<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $T=S+\{X\}$ and choose its [Gödel sentence](../../../../godel-sentence.md) $Z$, so $T\vdash Z\leftrightarrow\neg B_TZ$. The assumed reflection scheme gives the particular theorem

$$
T\vdash B_S(X\to Z)\to(X\to Z).
$$

The given extension-provability implication is $S\vdash B_TZ\to B_S(X\to Z)$. The fixed-point equivalence gives $T\vdash\neg Z\to B_TZ$, so these implications compose to

$$
T\vdash\neg Z\to(X\to Z).
$$

The supplied propositional [tautology](../../../../tautology.md) $((\neg Z\to(X\to Z))\to(X\to Z))$ gives $T\vdash X\to Z$, and $T\vdash X$ then yields $T\vdash Z$. The first of the [derivability conditions](../../../../hilbert-bernays-lob-derivability-conditions.md) for $T$ gives $T\vdash B_TZ$, while its Gödel equivalence gives $T\vdash\neg B_TZ$. Hence $T$ is inconsistent. By the [deduction theorem for propositional logic](../../../../deduction-theorem-for-propositional-logic.md),

$$
\boxed{S\vdash\neg X.}
$$

This proof uses diagonalization and proof transfer for the extension, and invokes neither [Löb's theorem](../../../../lob-s-theorem.md) nor the second incompleteness theorem.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Gödel's incompleteness theorems course of the University of Oxford](../../../split.md)
5. [Gödel's incompleteness theorems course of the University of Oxford](../../../../godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
