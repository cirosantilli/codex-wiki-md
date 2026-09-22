<h1 id="3a/solution">Solution</h1>

↑ **Parent:** [3A](../3a.md)

The parametrisation $r(x,y)=(x,y,F(x,y))$ has area factor

$$
|r_x\times r_y|=\sqrt{1+F_x^2+F_y^2},
$$

so $\operatorname{area}(S)=\iint_D\sqrt{1+F_x^2+F_y^2}\,dx\,dy$.

For the unbounded saddle $F=(x^2-y^2)/2$, this factor is $\sqrt{1+x^2+y^2}$. Thus the requested [integral](../../../../../integral.md) is

$$
2\pi\int_0^\infty\frac{r\,dr}{(1+r^2)^{3/2}}=2\pi,
$$

which converges because its radial tail is $O(r^{-2})$.

## ↑ Ancestors (10)

1. [3A](../3a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
