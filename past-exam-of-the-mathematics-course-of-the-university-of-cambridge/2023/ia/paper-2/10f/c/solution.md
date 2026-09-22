<h1 id="10f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An Erlang$(n,1)$ variable is a sum of $n$ independent rate-one exponential variables, each with mean and variance one. The central [limit](../../../../../../limit-of-a-function.md) theorem therefore gives

$$
\frac{X-n}{\sqrt n}\Rightarrow N(0,1).
$$

Consequently, for every fixed $q\geq0$,

$$
\boxed{\int_0^{n+q\sqrt n}\frac{x^{n-1}e^{-x}}{(n-1)!}dx
=\mathbb P\left(\frac{X-n}{\sqrt n}\leq q\right)
\longrightarrow\Phi(q).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
