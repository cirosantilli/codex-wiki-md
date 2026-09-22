<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A constant-coefficient [linear multistep method](../../../../linear-multistep-method-split.md), normalized so that $\alpha_k=1$, has the form

$$
\sum_{j=0}^k\alpha_jY_{n+j}=h\sum_{j=0}^k\beta_jf(x_{n+j},Y_{n+j}),\qquad x_n=x_0+nh.
$$

Here $Y_n$ approximates the solution $y(x_n)$ of the [initial value problem](../../../../initial-value-problem.md), and $Y_0,\ldots,Y_{k-1}$ are starting approximations. The coefficients are independent of $n$ and $h$. If $\beta_k=0$, the update is explicit; otherwise it is an [implicit time-stepping method](../../../../implicit-time-stepping-method.md), whose new value must satisfy the displayed equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../../numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
6. [MSc in mathematical modelling and scientific computing course of the University of Oxford](../../../../msc-in-mathematical-modelling-and-scientific-computing-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
