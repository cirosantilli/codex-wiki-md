<h1 id="26k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) states that if $(X_i)_{i\geq1}$ are [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with $\mathbb E|X_1|<\infty$, then

$$
\frac1n\sum_{i=1}^nX_i\longrightarrow\mathbb E X_1
$$

[almost surely](../../../../../../almost-sure-convergence.md). Under the stronger fourth-moment hypothesis, it has a short proof. Put $\mu=\mathbb EX_1$, $Y_i=X_i-\mu$, and $S_n=\sum_{i=1}^nY_i$. Independence and centering make every term in the expansion of $S_n^4$ vanish unless each index occurs at least twice, so

$$
\mathbb ES_n^4=n\mathbb EY_1^4+3n(n-1)(\mathbb EY_1^2)^2\leq Cn^2.
$$

For every $\varepsilon>0$, the [Markov inequality](../../../../../../markov-inequality.md) gives

$$
\mathbb P(|S_n|>\varepsilon n)\leq\frac{C}{\varepsilon^4n^2}.
$$

The probabilities are summable, so the first [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) says that $|S_n|>\varepsilon n$ occurs only finitely often almost surely. Apply this simultaneously to $\varepsilon=1,1/2,1/3,\ldots$ to obtain $S_n/n\to0$ almost surely, which is the claimed law.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26K](../../26k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
