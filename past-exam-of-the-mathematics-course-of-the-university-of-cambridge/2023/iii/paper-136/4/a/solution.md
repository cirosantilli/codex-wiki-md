<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Krasner's lemma](../../../../../../krasner-s-lemma.md) says that if $K$ is complete, $\alpha$ is separable over $K$, and

$$
|\beta-\alpha|<
\min_{\substack{\sigma(\alpha)\ne\alpha\\\sigma\in\operatorname{Gal}(\overline K/K)}}
|\alpha-\sigma(\alpha)|,
$$

then $K(\alpha)\subseteq K(\beta)$.

To prove it, let $\tau$ be an automorphism of $\overline K$ fixing $K(\beta)$. The absolute value has a unique extension to every finite extension of the complete field $K$, so it is invariant under $\tau$. If $\tau(\alpha)\ne\alpha$, the [ultrametric inequality](../../../../../../ultrametric-inequality.md) and the displayed strict inequality give

$$
|\tau(\alpha)-\beta|
=|\tau(\alpha)-\alpha|
>|\alpha-\beta|.
$$

But $\tau(\beta)=\beta$ and invariance gives $|\tau(\alpha)-\beta|=|\alpha-\beta|$, a contradiction. Every automorphism fixing $K(\beta)$ therefore fixes $\alpha$, which proves the field inclusion by [Galois correspondence](../../../../../../galois-correspondence.md).

Now let $L/\mathbb Q_p$ be finite. By the [primitive element theorem](../../../../../../primitive-element-theorem.md), write $L=\mathbb Q_p(\alpha)$ with separable minimal polynomial $f\in\mathbb Q_p[X]$. Approximate the coefficients of $f$ closely by those of a polynomial $g\in\mathbb Q[X]$ of the same degree. [Continuity of roots over a non-Archimedean field](../../../../../../continuity-of-roots-over-a-non-archimedean-field.md) gives a root $\beta$ of $g$ arbitrarily close to $\alpha$. Choose it close enough for [Krasner's lemma](../../../../../../krasner-s-lemma.md); then

$$
\mathbb Q_p(\alpha)\subseteq\mathbb Q_p(\beta).
$$

The degree bound from $\deg g=\deg f$ forces equality. If $F=\mathbb Q(\beta)$ and $\mathfrak p$ is the prime selected by the embedding $F\hookrightarrow\overline{\mathbb Q}_p$, its completion is

$$
F_{\mathfrak p}\cong\mathbb Q_p(\beta)=L.
$$

**Thus every finite extension of $\mathbb Q_p$ is the [completion of a number field at a prime ideal](../../../../../../completion-of-a-number-field-at-a-prime-ideal.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
