# Type (information theory)

↑ **Parent:** [Information theory](information-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_(information_theory))

A [type](type-information-theory.md) summarizes a string by how often each symbol occurs. Fix a finite [alphabet](alphabet.md) $\mathcal A$ of [cardinality](cardinality.md) $m$ and a positive length $n$. For a string $x^n=(x_1,\ldots,x_n)$, its [empirical distribution](type-information-theory.md) is the [probability mass function](probability-mass-function.md)

$$
\widehat q_{x^n}(a)=\frac{\#\{j:x_j=a\}}{n},\qquad a\in\mathcal A.
$$

The [empirical distribution](type-information-theory.md) forgets order. The strings $0011$ and $1010$ both assign [probability](probability.md) $1/2$ to each binary symbol; $0001$ assigns $3/4$ to zero and $1/4$ to one. Thus a long string can have a short summary even though that summary does not reconstruct the original order.

For [independent and identically distributed](independent-and-identically-distributed-random-variables.md) symbols, this loss of order has a useful consequence: all strings with the same [empirical distribution](type-information-theory.md) have the same [probability](probability.md). The [method of types](method-of-types.md) uses this symmetry to turn questions about exponentially many strings into counting questions about relatively few frequency profiles.[§I, printed p. 2505: partition by empirical distribution and equiprobability under a memoryless model](the-method-of-types-by-imre-csiszar.md)

**Table of contents**

- [Type class](type-class.md)
  - [Size of a type class](size-of-a-type-class.md)
  - [Indexing within a type class](indexing-within-a-type-class.md)
- [Method of types](method-of-types.md)
  - [Number of empirical types](number-of-empirical-types.md)
  - [Entropy bounds for a type class](entropy-bounds-for-a-type-class.md)
  - [Probability of a type class](probability-of-a-type-class.md)
  - [Development of the method of types](development-of-the-method-of-types.md)
  - [Sanov theorem](sanov-theorem.md)
  - [Information projection](information-projection.md)
    - [Information projection on three outcomes](information-projection-on-three-outcomes.md)
      - [Information projection and Euclidean projection](information-projection-and-euclidean-projection.md)
    - [Uniform-reference information projection maximizes entropy](uniform-reference-information-projection-maximizes-entropy.md)
    - [Pythagorean inequality for information projection](pythagorean-inequality-for-information-projection.md)
    - [Relative entropy minimization under a mean constraint](relative-entropy-minimization-under-a-mean-constraint.md)
      - [Information projection and rare sample means](information-projection-and-rare-sample-means.md)
    - [Historical source for information projection](historical-source-for-information-projection.md)

## ↑ Ancestors (5)

1. [Information theory](information-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-224/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-224/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/2/d/solution.md)
- [Type (information theory)](type-information-theory.md)
