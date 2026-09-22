<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Assume first that no two members of the [uniform set family](../../../../../../uniform-set-family.md) $\mathcal A\subseteq[n]^{(k)}$ meet in exactly one point. Fix $A_0\in\mathcal A$. Since $\mathcal A$ is an [intersecting family](../../../../../../intersecting-family.md), every $B\in\mathcal A$ then contains at least two elements of $A_0$. Consequently

$$
|\mathcal A|
\leq\binom{k}{2}\binom{n-2}{k-2}
=O(n^{k-2})
=o\left(\binom{n-1}{k-1}\right).
$$

This proves the stated dichotomy.

If the small alternative holds, then for sufficiently large $n$ any fixed $i$ has all but at most $\varepsilon\binom{n-1}{k-1}$ members of $\mathcal A$ containing it. Otherwise choose $A,B\in\mathcal A$ with $A\cap B=\{i\}$. Every $C\in\mathcal A$ not containing $i$ must meet both $A\setminus\{i\}$ and $B\setminus\{i\}$, so

$$
|\{C\in\mathcal A:i\notin C\}|
\leq(k-1)^2\binom{n-2}{k-2}
=o\left(\binom{n-1}{k-1}\right).
$$

For sufficiently large $n$ this is at most $\varepsilon\binom{n-1}{k-1}$, as required.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
