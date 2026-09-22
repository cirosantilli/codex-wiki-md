<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Using the causal [Green's function](../../../../../green-s-function-split.md),

$$
y_p(x)=\int_0^xG(x,\xi)\xi\,d\xi=x^r\int_0^x\xi^{2-r}\log(x/\xi)\,d\xi.
$$

Put $\xi=xs$. Since $\alpha>-5$ is equivalent to $r<3$, the [improper integral](../../../../../improper-integral.md) converges and gives

$$
y_p(x)=x^3\int_0^1s^{2-r}(-\log s)\,ds=\frac{x^3}{(3-r)^2}=\boxed{\frac{4x^3}{(\alpha+5)^2}.}
$$

The elementary identity $\int_0^1s^{p-1}(-\log s)ds=1/p^2$ follows by differentiating $\int_0^1s^{p-1}ds=1/p$ for $p>0$. Direct substitution checks $L(x^3)=(\alpha+5)^2x/4$, and the displayed solution and its first [derivative](../../../../../derivative.md) vanish at zero.

To give all solutions allowed by the printed [boundary conditions](../../../../../boundary-condition.md), retain the singular-endpoint qualification from part (b):

$$
\boxed{y(x)=\begin{cases}\dfrac{4x^3}{(\alpha+5)^2}+x^{(1-\alpha)/2}(C_1+C_2\log x),&-5<\alpha<-1,\\\dfrac{4x^3}{(\alpha+5)^2},&\alpha\geq-1.\end{cases}}
$$

Thus the causal integral gives a particular member of a two-parameter family in the first range and the unique solution in the second.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
