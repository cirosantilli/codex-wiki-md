<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\lambda_n=\alpha n+\beta$,

$$
\sum_{n=0}^{\infty}\frac1{\alpha n+\beta}=\infty,
$$

so part (b) ensures nonexplosion. The [Markov jump-process generator](../../../../../../markov-jump-process-generator.md) acts on the identity function $f(n)=n$ as

$$
(Lf)(n)=(\alpha n+\beta)\bigl((n+1)-n\bigr)
=\alpha n+\beta.
$$

Consequently $m(t)=\mathbb EN(t)$ satisfies

$$
m'(t)=\mathbb E[(Lf)(N(t))]
=\alpha m(t)+\beta,
\qquad m(0)=0.
$$

Solving this linear [ordinary differential equation](../../../../../../ordinary-differential-equation.md) gives the mean of the [linear birth process with immigration](../../../../../../linear-birth-process-with-immigration.md):

$$
\boxed{\mathbb EN(t)=\frac{\beta}{\alpha}(e^{\alpha t}-1)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
