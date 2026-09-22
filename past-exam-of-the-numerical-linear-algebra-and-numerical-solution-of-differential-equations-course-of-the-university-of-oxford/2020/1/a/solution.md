<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the increment function of the [one-step method](../../../../one-step-method.md) as $\Phi(x,v,h)=f(x+\beta h,v+\beta h f(x,v))$. Its [consistency error](../../../../normalized-local-truncation-error.md) is

$$
T_n=\frac{y(x_n+h)-y(x_n)}h-\Phi(x_n,y(x_n),h).
$$

As $h\to0$, the first term tends to $y'(x_n)$ and the second tends to $f(x_n,y(x_n))=y'(x_n)$ by [continuity](../../../../continuous-function.md). Both limits are uniform along the exact-solution curve, a [compact set](../../../../compact-space.md): its small stage perturbations lie in a fixed compact neighborhood, so [uniform continuity](../../../../uniform-continuity.md) applies there. Thus $\max_{n<N}|T_n|\to0$, proving **consistency for every $\beta\in[0,1]$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../../numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
6. [MSc in mathematical modelling and scientific computing course of the University of Oxford](../../../../msc-in-mathematical-modelling-and-scientific-computing-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
