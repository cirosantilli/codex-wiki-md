<h1 id="28j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A simple birth process with parameter $\lambda$ starting from one individual is the [Yule process](../../../../../../yule-process.md): when its population is $n$, it waits an exponential time of rate $n\lambda$ and then moves to $n+1$.

For $f(n)=n$, the [Markov jump-process generator](../../../../../../markov-jump-process-generator.md) satisfies

$$
(Lf)(n)=n\lambda\bigl(f(n+1)-f(n)\bigr)=n\lambda.
$$

Therefore $\mu(t)=\mathbb E X_t$ obeys

$$
\mu'(t)=\lambda\mu(t),
\qquad \mu(0)=1.
$$

It follows, as recorded by the [mean population of a Yule process](../../../../../../mean-population-of-a-yule-process.md), that

$$
\boxed{\mathbb E X_t=e^{\lambda t}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
