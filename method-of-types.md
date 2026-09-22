# Method of types

↑ **Parent:** [Type (information theory)](type-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_types)

The [method of types](method-of-types.md) combines two facts: there are few possible [empirical distributions](type-information-theory.md), and strings within each [type class](type-class.md) are equiprobable under an [independent and identically distributed](independent-and-identically-distributed-random-variables.md) source. [Information entropy](information-entropy-split.md) determines how many strings share a frequency profile; [relative entropy](kullback-leibler-divergence.md) determines how unlikely that profile is under a specified source law. The connection is useful both for [lossless source coding](lossless-source-coding.md) and for understanding rare observations.

The following formulas use [natural logarithms](natural-logarithm.md), so [information entropy](information-entropy-split.md) and [relative entropy](kullback-leibler-divergence.md) are measured in [nats](nat-unit.md). Define

$$
H_e(q)=-\sum_a q(a)\ln q(a),\qquad
D_e(q\Vert p)=\sum_a q(a)\ln\frac{q(a)}{p(a)}.
$$

Here $p$ is the source [probability mass function](probability-mass-function.md) and $q$ is an attainable [empirical distribution](type-information-theory.md). Use $0\ln0=0$; first assume every $p(a)>0$. Base-two [logarithms](logarithm.md) give the equivalent formulas with $2^{nH_2(q)}$ and $2^{-nD_2(q\Vert p)}$.

**Table of contents**

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

## ↑ Ancestors (6)

1. [Type (information theory)](type-information-theory.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Development of the method of types](development-of-the-method-of-types.md)
- [Information projection and rare sample means](information-projection-and-rare-sample-means.md)
- [Method of types](method-of-types.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-224/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-224/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-224/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-224/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/2/d/solution.md)
- [Type (information theory)](type-information-theory.md)
