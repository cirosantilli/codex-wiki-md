<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any partition of $[0,t]$,

$$
f(t)^2-f(0)^2
=2\sum_k f(t_{k-1})(f(t_k)-f(t_{k-1}))
+\sum_k(f(t_k)-f(t_{k-1}))^2.
$$

The final sum is at most the largest increment of $f$ times its total variation. It tends to zero because $f$ is uniformly continuous. Part b then gives the integration-by-parts identity

$$
2\int_0^tf(s)\,df(s)=f(t)^2-f(0)^2.
$$

**Thus the formula stated in the question holds when $f(0)=0$; for a general initial value the necessary endpoint correction is $-f(0)^2$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
