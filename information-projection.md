# Information projection

↑ **Parent:** [Method of types](method-of-types.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Information_projection)

An [information projection](information-projection.md) chooses the [probability distribution](probability-distribution-split.md) that satisfies a constraint while departing least from a reference law in [relative entropy](kullback-leibler-divergence.md). The constraint might specify an [expected value](expected-value-split.md), several marginal [probability distributions](probability-distribution-split.md), or another [convex set](convex-set-split.md) of permissible laws. The reference is held fixed: the variable is the first argument of $D(q\Vert p)$. Reversing the arguments gives a different minimization problem.

For a finite [alphabet](alphabet.md) $\mathcal A$, take a positive reference [probability mass function](probability-mass-function.md) $p(a)>0$ and a nonempty closed [convex set](convex-set-split.md) $\mathcal C$ in the [probability simplex](probability-simplex.md). Then

$$
\boxed{q^*=\arg\min_{q\in\mathcal C}D(q\Vert p),\qquad
D(q\Vert p)=\sum_{a:q(a)>0}q(a)\ln\frac{q(a)}{p(a)}.}
$$

The minimum exists and its minimizing [probability distribution](probability-distribution-split.md) is unique. In this article, [natural logarithms](natural-logarithm.md) give [nats](nat-unit.md). Using base-two [logarithms](logarithm.md) rescales the objective without changing the minimizer.[§3, printed pp. 440–441: finite-alphabet information projection onto a closed convex set](information-theory-and-statistics-a-tutorial-by-imre-csiszar-and-paul-c-shields.md)

If $p$ already meets the constraint, its [information projection](information-projection.md) is $p$ itself by [relative entropy nonnegativity](relative-entropy-nonnegativity.md). If not, a constraint can change the relative weights of outcomes without specifying every weight individually. [Relative entropy minimization under a mean constraint](relative-entropy-minimization-under-a-mean-constraint.md) gives an especially useful example: it tilts the reference law rather than choosing an arbitrary distribution with the right average.

**Table of contents**

- [Information projection on three outcomes](information-projection-on-three-outcomes.md)
  - [Information projection and Euclidean projection](information-projection-and-euclidean-projection.md)
- [Uniform-reference information projection maximizes entropy](uniform-reference-information-projection-maximizes-entropy.md)
- [Pythagorean inequality for information projection](pythagorean-inequality-for-information-projection.md)
- [Relative entropy minimization under a mean constraint](relative-entropy-minimization-under-a-mean-constraint.md)
  - [Information projection and rare sample means](information-projection-and-rare-sample-means.md)
- [Historical source for information projection](historical-source-for-information-projection.md)

## ↑ Ancestors (7)

1. [Method of types](method-of-types.md)
2. [Type (information theory)](type-information-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Historical source for information projection](historical-source-for-information-projection.md)
- [Information projection](information-projection.md)
- [Information projection and Euclidean projection](information-projection-and-euclidean-projection.md)
- [Information projection on three outcomes](information-projection-on-three-outcomes.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-224/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/2/c/solution.md)
- [Pythagorean inequality for information projection](pythagorean-inequality-for-information-projection.md)
- [Uniform-reference information projection maximizes entropy](uniform-reference-information-projection-maximizes-entropy.md)
