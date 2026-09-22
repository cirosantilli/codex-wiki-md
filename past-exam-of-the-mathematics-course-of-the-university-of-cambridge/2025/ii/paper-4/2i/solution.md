<h1 id="2i/solution">Solution</h1>

↑ **Parent:** [2I](../2i.md)

Starting with $x_0=x>0$, the [continued-fraction algorithm](../../../../../continued-fraction-algorithm.md) sets

$$
a_n=\lfloor x_n\rfloor,
\qquad
x_{n+1}=\frac1{x_n-a_n}
$$

unless $x_n$ is already an integer. This gives

$$
x=[a_0;a_1,a_2,\ldots].
$$

Every finite continued fraction is rational, since it is built from integers by finitely many additions and reciprocals. Conversely, if $x=p/q$ is rational in lowest terms, then

$$
\frac pq=a_0+\frac rq,
\qquad 0\leq r<q.
$$

When $r\ne0$, the next complete quotient is $q/r$. Thus each step is an application of the Euclidean algorithm and replaces the denominator by a smaller nonnegative remainder. The process must terminate. This proves the [termination criterion for a simple continued fraction](../../../../../termination-criterion-for-a-simple-continued-fraction.md).

For $x=\sqrt3$,

$$
a_0=1,\qquad
x_1=\frac1{\sqrt3-1}=\frac{\sqrt3+1}{2},\qquad a_1=1,
$$

and

$$
x_2=\frac1{x_1-1}=\sqrt3+1,\qquad a_2=2.
$$

Finally,

$$
x_3=\frac1{x_2-2}=\frac1{\sqrt3-1}=x_1,
$$

so the complete quotients repeat. Hence the [continued fraction of the square root of three](../../../../../continued-fraction-of-the-square-root-of-three.md) is

$$
\boxed{\sqrt3=[1;\overline{1,2}]}.
$$

## ↑ Ancestors (10)

1. [2I](../2i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
