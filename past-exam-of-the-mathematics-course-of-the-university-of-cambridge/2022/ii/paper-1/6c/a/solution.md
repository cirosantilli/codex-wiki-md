<h1 id="6c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The positive fixed point satisfies $x_*=x_*e^{r(1-x_*)}$, hence $x_*=1$. Put $x_n=1+u_n$ and retain first-order terms:

$$
1+u_{n+1}=(1+u_n)e^{-ru_{n-1}}
=1+u_n-ru_{n-1}+O(u^2).
$$

Thus

$$
\boxed{u_{n+1}=u_n-ru_{n-1}},
$$

with characteristic polynomial $\lambda^2-\lambda+r$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6C](../../6c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
