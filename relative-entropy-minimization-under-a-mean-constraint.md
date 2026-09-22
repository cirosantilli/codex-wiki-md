# Relative entropy minimization under a mean constraint

↑ **Parent:** [Information projection](information-projection.md)

Let $p_i>0$ be a [probability mass function](probability-mass-function.md) on a finite [alphabet](alphabet.md) with numerical outcomes $a_i$. Prescribe a [mean](expected-value-split.md) $m$ strictly between the smallest and largest outcomes. [Exponential tilting](exponential-tilting.md) gives

$$
q_i^*=\frac{p_i e^{\theta a_i}}{Z(\theta)},\qquad
Z(\theta)=\sum_jp_j e^{\theta a_j},
$$

with $\theta$ chosen so that $\sum_iq_i^*a_i=m$. For any other feasible law $r$, direct substitution yields

$$
D(r\Vert p)=D(r\Vert q^*)+\theta m-\ln Z(\theta),\qquad
D(q^*\Vert p)=\theta m-\ln Z(\theta).
$$

[Relative entropy nonnegativity](relative-entropy-nonnegativity.md) therefore proves optimality and uniqueness. At an extreme prescribed [mean](expected-value-split.md), feasible laws may have zero [probabilities](probability.md); a finite tilting parameter need not realize them, although a limit can.

**Table of contents**

- [Information projection and rare sample means](information-projection-and-rare-sample-means.md)

## ↑ Ancestors (8)

1. [Information projection](information-projection.md)
2. [Method of types](method-of-types.md)
3. [Type (information theory)](type-information-theory.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Information projection](information-projection.md)
- [Pythagorean inequality for information projection](pythagorean-inequality-for-information-projection.md)
