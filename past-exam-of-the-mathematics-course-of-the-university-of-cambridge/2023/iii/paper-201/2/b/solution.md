<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $A_n=\{X_m=0\text{ for some }m\geq n\}$. By the [Markov property](../../../../../../markov-property.md),

$$
v(X_n)=\mathbb P(A_n\mid\mathcal F_n).
$$

The events $A_n$ decrease to the event that the walk visits zero infinitely often, which has probability zero by the stated transience assumption. Hence

$$
\mathbb E[v(X_n)]=\mathbb P(A_n)\longrightarrow0.
$$

Part a and the [almost sure supermartingale convergence theorem](../../../../../../almost-sure-supermartingale-convergence-theorem.md) give an almost-sure limit $V\geq0$. By [Fatou lemma](../../../../../../fatou-s-lemma.md), $\mathbb EV\leq\liminf_n\mathbb E[v(X_n)]=0$, so $V=0$ almost surely.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
