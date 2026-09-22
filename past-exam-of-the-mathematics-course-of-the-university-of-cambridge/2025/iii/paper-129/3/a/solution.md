<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One standard normalized form of the [Croot-Sisask almost-periodicity theorem](../../../../../../croot-sisask-almost-periodicity-theorem.md) is this. Let $A,S$ be finite subsets of an abelian group with $|A+S|\leq K|A|$, let $q\geq2$, let $0<\epsilon<1$, and let $f$ be a complex function. There is $T\subseteq S$ with

$$
|T|\geq(2K)^{-O(q/\epsilon^2)}|S|
$$

such that every $t\in T-T$ satisfies

$$
\|\tau_t(1_A*f)-1_A*f\|_{L^q}
\leq\epsilon\|1_A\|_{L^1}\|f\|_{L^q}.
$$

For the proof, sample $k=O(q/\epsilon^2)$ independent points of $A$ and approximate $1_A*f$ by the empirical average of the corresponding translates of $f$. A moment inequality bounds the expected $L^q$ error, so many samples are good. The small size of $A+S$ lets a translation and pigeonhole argument find many shifts in $S$ producing the same good approximation. Subtracting two such shifts and applying the [triangle inequality](../../../../../../triangle-inequality.md) yields the almost periods in $T-T$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
