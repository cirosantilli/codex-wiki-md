<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove the [Doob-Dynkin lemma](../../../../../doob-dynkin-lemma.md) here by [simple function](../../../../../simple-function.md) approximation. Choose $C<\infty$ such that $|Z|\leq C$ everywhere, and let

$$
Z_m=2^{-m}\lfloor2^mZ\rfloor.
$$

Each $Z_m$ is a finite-valued $\sigma(X)$-[measurable function](../../../../../measurable-function.md) and $Z_m\to Z$ pointwise. Write its level [sets](../../../../../set-split.md) as $A_{m,j}$, with associated values $z_{m,j}$. By part (i), choose [Borel sets](../../../../../borel-set.md) $D_{m,j}$ with $A_{m,j}=X^{-1}(D_{m,j})$. Define the [Borel measurable functions](../../../../../borel-measurable-function.md)

$$
g_m(x)=\sum_jz_{m,j}\mathbf1_{D_{m,j}}(x).
$$

Although the chosen $D_{m,j}$ need not partition all of $\mathbb R$, their [inverse images](../../../../../preimage.md) do partition $\Omega$, so $g_m(X)=Z_m$ exactly.

Apply [scalar clipping](../../../../../scalar-clipping.md) to each $g_m$ with bounds $[-C-1,C+1]$, preserving this equality, and define $g(x)=\limsup_mg_m(x)$. A bounded [limit superior](../../../../../limit-superior.md) of [Borel measurable functions](../../../../../borel-measurable-function.md) is a finite [Borel measurable function](../../../../../borel-measurable-function.md). At every $\omega\in\Omega$ the [limit of a sequence](../../../../../limit-of-a-sequence.md) exists and gives

$$
\boxed{g(X(\omega))=\lim_mZ_m(\omega)=Z(\omega).}
$$

Thus the factorization is exact for a bounded, exactly $\sigma(X)$-[measurable function](../../../../../measurable-function.md). If hypotheses are instead given only up to [null sets](../../../../../null-set.md), the corresponding conclusion is a factorization holding [almost surely](../../../../../almost-sure-convergence.md) after choosing a representative.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
