<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One strong form of [Hensel lemma](../../../../../../hensel-s-lemma.md) is this: if $K$ is complete for a [discrete valuation](../../../../../../discrete-valuation.md) $v$, $f\in\mathcal O_K[X]$, and $a_0\in\mathcal O_K$ satisfies

$$
v(f(a_0))>2v(f'(a_0)),
$$

then there is a unique root $\alpha$ satisfying

$$
v(\alpha-a_0)>v(f'(a_0)).
$$

Define the [Newton iteration over a valued field](../../../../../../newton-iteration-over-a-valued-field.md)

$$
a_{n+1}=a_n-\frac{f(a_n)}{f'(a_n)}.
$$

Taylor expansion and the [ultrametric inequality](../../../../../../ultrametric-inequality.md) show inductively that $v(f'(a_n))=v(f'(a_0))$ and

$$
v(f(a_{n+1}))\geq2v(f(a_n))-2v(f'(a_0)).
$$

Thus the valuations of the corrections $a_{n+1}-a_n$ tend to infinity, so $(a_n)$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md). [Completeness](../../../../../../completeness.md) gives a limit $\alpha$, and [continuity](../../../../../../continuous-function.md) gives $f(\alpha)=0$. If $\beta$ is another root in the stated ball, Taylor expansion of $f(\beta)-f(\alpha)$ shows that the linear term has strictly smaller valuation than all higher terms unless $\beta=\alpha$, proving uniqueness.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
