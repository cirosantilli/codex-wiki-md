<h1 id="29l/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $r=e^\theta$. The geometric moments are

$$
m:=\mathbb EY_i=\frac1{r-1},\qquad
\operatorname{Var}(Y_i)=\frac r{(r-1)^2}.
$$

For $g(y)=\log((1+y)/y)$, one has $g(m)=\theta$ and

$$
g'(m)=-\frac1{m(1+m)}=-\frac{(r-1)^2}{r}.
$$

The central [limit](../../../../../../../limit-of-a-function.md) theorem for $\overline Y$ followed by the [delta method](../../../../../../../delta-method.md) therefore gives

$$
\boxed{\sqrt n(\widetilde\theta_n-\theta)Rightarrow
N\left(0,\frac{(e^\theta-1)^2}{e^\theta}\right).}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [29L](../../../29l.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
