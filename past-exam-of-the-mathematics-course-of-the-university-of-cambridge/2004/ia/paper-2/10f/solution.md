<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

For [events](../../../../../event.md) with $\mathbb P(B)>0$, the [conditional probability](../../../../../conditional-probability.md) is

$$
\boxed{\mathbb P(A\mid B)=\frac{\mathbb P(A\cap B)}{\mathbb P(B)}.}
$$

Use the [sample space](../../../../../sample-space.md) $\Omega=\{1,2,3,4\}\times\{0,1\}^4$, where the first coordinate is the chosen coin and the other coordinates record which of its two physically distinguished faces lands upwards on each toss. There are $4\cdot16=64$ equally likely elementary outcomes. Label the double-headed coin by one. For that coin both face indices mean heads; for each other coin only face index one means heads. In particular, strings of observed heads and tails are not equally likely outcomes.

Let $E$ be the [event](../../../../../event.md) that the first three tosses show heads. With coin one all sixteen face-index strings are permitted. For each ordinary coin the first three indices must be one and the fourth is free, giving two strings. Thus $|E|=16+3\cdot2=22$. Of these outcomes, sixteen from the double-headed coin and one from each ordinary coin also have a fourth head. Hence

$$
\boxed{\mathbb P(\text{fourth head}\mid E)=\frac{16+3}{22}=\frac{19}{22}.}
$$

Equivalently, [Bayes' theorem](../../../../../bayes-theorem.md) gives [conditional probability](../../../../../conditional-probability.md) $8/11$ of having selected the double-headed coin after $E$; the fourth-head [probability](../../../../../probability.md) is then $8/11+(3/11)(1/2)=19/22$. The tosses are [independent](../../../../../independent-random-variables.md) conditional on the selected coin, while mixing over the same coin explains their unconditional dependence.

## ↑ Ancestors (11)

1. [10F](../10f.md)
2. [Section II](../section-ii.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
