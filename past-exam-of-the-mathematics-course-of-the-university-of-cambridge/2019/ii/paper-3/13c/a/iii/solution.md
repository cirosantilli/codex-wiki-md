<h1 id="13c/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The normalized ansatz intended in the question is

$$
\phi(s,t)=\exp\bigl((s-1)f(t)\bigr),
$$

for which $\phi(1,t)=1$. Substitution into the equation from part (ii) and cancellation of $(s-1)\phi$ gives the [linear ordinary differential equation](../../../../../../../linear-ordinary-differential-equation.md)

$$
f'=\lambda-\beta f.
$$

Thus

$$
f(t)=\frac\lambda\beta+\left(f(0)-\frac\lambda\beta\right)e^{-\beta t}.
$$

This generating function is that of a [Poisson distribution](../../../../../../../poisson-distribution.md) with parameter $f(t)$. Equivalently, differentiating at $s=1$ gives

$$
\langle n\rangle=\partial_s\phi(1,t)=f(t),
\qquad
\sigma^2=\partial_s^2\phi(1,t)+\partial_s\phi(1,t)-\partial_s\phi(1,t)^2=f(t).
$$

Consequently

$$
\boxed{\langle n\rangle\longrightarrow\frac\lambda\beta,
\qquad \sigma^2\longrightarrow\frac\lambda\beta.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [13C](../../../13c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
