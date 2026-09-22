<h1 id="12f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Evaluation of the [probability generating function](../../../../../../probability-generating-function.md) at zero selects the constant coefficient, so

$$
\boxed{\mathbb P(X_n=0)=G_n(0)=1-\alpha^{(1-\beta^n)/(1-\beta)}\longrightarrow1-\alpha^{1/(1-\beta)}.}
$$

To identify this limit with ultimate extinction, let $E_n=\{X_n=0\}$. The absorbing-zero property of the [branching process](../../../../../../branching-process.md) gives $E_n\subseteq E_{n+1}$. Ultimate extinction means that some finite generation is empty, namely $E=\bigcup_{n\ge0}E_n$. Continuity of [probability](../../../../../../probability.md) on increasing [events](../../../../../../event.md) therefore gives

$$
\boxed{\mathbb P(E)=\lim_{n\to\infty}\mathbb P(E_n)=1-\alpha^{1/(1-\beta)}.}
$$

This set argument is essential: it uses absorption, rather than inferring extinction merely from a numerical limit of generation probabilities.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
