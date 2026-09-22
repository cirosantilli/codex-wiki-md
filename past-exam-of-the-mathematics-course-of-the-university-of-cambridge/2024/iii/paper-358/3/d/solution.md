<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume for contradiction that a sequence of general algorithms $\Gamma_n$ decides ergodicity from the perfect measurement data, so that $\Gamma_n(F)$ eventually equals $\Xi_{\rm erg}(F)$ for every $F\in\Omega$.

Restrict the input class to the circle rotations

$$
F_a(x)=x+a\pmod{2\pi}.
$$

From [inexact information in the SCI hierarchy](../../../../../../inexact-information-in-the-sci-hierarchy.md) for the real number $a$, one can answer every requested measurement of $F_a(x)$ to the same precision. The supposed algorithms would therefore give a one-limit decision procedure for

$$
a\longmapsto\mathbf1_{\mathbb R\setminus\mathbb Q}(a/\pi),
$$

because part (b)(ii) identifies ergodicity with irrationality.

Every finite-information general algorithm is locally constant on a sufficiently small cylinder of the inexact data. A pointwise limit of a sequence of such functions is a [Baire class one function](../../../../../../baire-class-one-function.md). But the rationality indicator is discontinuous at every real number: every interval contains both rational and irrational numbers. The theorem that the discontinuity set of a Baire class one function is meagre, or directly [rationality indicator is not Baire class one](../../../../../../rationality-indicator-is-not-baire-class-one.md), gives a contradiction.

Hence no one-limit tower of general algorithms can decide ergodicity, even with the perfect measurement device:

$$
\boxed{
\{\Xi_{\rm erg},\Omega,\{0,1\},\Lambda\}^{\Delta_1}
\notin\Delta_2^G.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
