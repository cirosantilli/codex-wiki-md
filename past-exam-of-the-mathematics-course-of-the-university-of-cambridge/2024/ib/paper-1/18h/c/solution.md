<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [power function of a statistical test](../../../../../../power-function-of-a-statistical-test.md) for Test 1 is

$$
\boxed{
\pi_1(\theta)=
\begin{cases}
0,&\theta\leq-0.05,\\
\theta+0.05,&-0.05<\theta<0.95,\\
1,&\theta\geq0.95.
\end{cases}}
$$

Put $a=1/\sqrt{10}$. Test 2 rejects when

$$
U_1+U_2>2-a-2\theta.
$$

Using the two branches of the triangular distribution gives

$$
\boxed{
\pi_2(\theta)=
\begin{cases}
0,&\theta\leq-a/2,\\
\frac12(a+2\theta)^2,
&-a/2<\theta<(1-a)/2,\\
1-\frac12(2-a-2\theta)^2,
&(1-a)/2\leq\theta<(2-a)/2,\\
1,&\theta\geq(2-a)/2.
\end{cases}}
$$

Both [functions](../../../../../../function-split.md) equal $0.05$ at the least favourable null value $\theta=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
