<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [type](../../../../../../type-information-theory.md) of $x_1^n\in A^n$ is its [empirical distribution](../../../../../../type-information-theory.md)

$$
\widehat P_{x_1^n}(a)=\frac1n\sum_{i=1}^n\mathbf1_{\{x_i=a\}},
\qquad a\in A.
$$

Its [type class](../../../../../../type-class.md) is

$$
T(P)=\{y_1^n\in A^n:\widehat P_{y_1^n}=P\}.
$$

Every string in $T(P)$ has $Q^n$-probability

$$
\prod_{a\in A}Q(a)^{nP(a)}
=2^{-n\{H(P)+D(P\Vert Q)\}},
$$

while the [method of types](../../../../../../method-of-types.md) gives $|T(P)|\leq2^{nH(P)}$. Therefore

$$
\boxed{Q^n(T(P))\leq2^{-nD(P\Vert Q)}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
