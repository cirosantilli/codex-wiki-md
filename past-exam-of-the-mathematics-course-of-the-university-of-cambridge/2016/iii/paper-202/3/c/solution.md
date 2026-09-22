<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The [Girsanov theorem](../../../../../../girsanov-theorem.md) construction proves a [weak stochastic solution](../../../../../../weak-solution-of-a-stochastic-differential-equation.md), but does not by itself establish a [strong stochastic solution](../../../../../../strong-solution-of-a-stochastic-differential-equation.md).** It constructs $X=x+W$ first, and then constructs a new driving [Brownian motion](../../../../../../brownian-motion-split.md) $B=W-\int b(X_s)ds$. Adaptation of $X$ to the original [filtration](../../../../../../filtration-probability-theory.md) of $W$ does not by itself prove adaptation to the smaller [natural filtration](../../../../../../natural-filtration.md) of $B$. Inverting this relation requires an additional result; [uniqueness in law](../../../../../../uniqueness-in-law.md) alone is insufficient in general.

**For the particular coefficients in part (b), however, the literal claim that a strong solution may fail is incorrect.** The [strong existence theorem for additive-noise SDEs with bounded measurable drift](../../../../../../strong-existence-theorem-for-additive-noise-sdes-with-bounded-measurable-drift.md) gives [strong existence](../../../../../../strong-existence.md) and [pathwise uniqueness](../../../../../../pathwise-uniqueness.md) for bounded Borel state-dependent $b$ and unit diffusion. Consequently every weak realization here is determined by its driving noise and initial value. This theorem is deeper than the [Girsanov theorem](../../../../../../girsanov-theorem.md) argument and no proof is needed here. Examples with path-dependent drift or with a nonconstant diffusion coefficient do not contradict it.

The valid distinction is therefore: the argument in part (b) has established weak existence and [uniqueness in law](../../../../../../uniqueness-in-law.md); strong existence requires an additional theorem, and in this class that theorem is available. A primary reference for the correction is [On strong solutions and explicit formulas for solutions of stochastic integral equations](https://www.mathnet.ru/php/archive.phtml?jrnid=sm&option_lang=eng&paperid=2601&wshow=paper).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
