<h1 id="section-g/31/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a chosen bead, the uniform displacement cube is inversion symmetric, so the [proposal distribution](../../../../../../proposal-distribution.md) satisfies $q(X\to Y)=q(Y\to X)$. The target canonical density is $\pi(X)\propto\exp[-\beta U(X)]$ for allowed configurations. With $a(X,Y)=\min[1,e^{-\beta(U(Y)-U(X))}]$,

$$
\boxed{\pi(X)q(X,Y)a(X,Y)=q(X,Y)\min[\pi(X),\pi(Y)]=\pi(Y)q(Y,X)a(Y,X).}
$$

This proves [detailed balance](../../../../../../detailed-balance.md). Overlapping trials have zero target weight and are rejected. The proposal must retain rejected trials as self-transitions; repeatedly proposing until a nonoverlapping move appears would generally introduce a configuration-dependent proposal normalization and need a Hastings correction. [Detailed balance](../../../../../../detailed-balance.md) establishes stationarity, while sufficient sampling also requires practical exploration of the accessible state space.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [31](../../31.md)
3. [Section G](../../../section-g.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
