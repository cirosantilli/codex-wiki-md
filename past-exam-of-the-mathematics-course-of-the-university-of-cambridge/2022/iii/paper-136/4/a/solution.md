<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One strong form of the [Hensel lemma](../../../../../../hensel-s-lemma.md) is this: if a complete discretely valued field $K$, a polynomial $f\in\mathcal O_K[X]$, and $a\in\mathcal O_K$ satisfy

$$
v(f(a))>2v(f'(a)),
$$

then there is a unique root $\alpha$ in the ball $v(\alpha-a)>v(f'(a))$.

Set $a_{n+1}=a_n-f(a_n)/f'(a_n)$. Taylor expansion shows that the valuation of the error at least doubles at each step, while $v(f'(a_n))$ remains constant. Thus the corrections tend to zero geometrically, so completeness gives a limit $\alpha$. Continuity gives $f(\alpha)=0$. Applying the same Taylor estimate to two roots in the stated ball proves uniqueness. This is [Newton iteration over a valued field](../../../../../../newton-iteration-over-a-valued-field.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
