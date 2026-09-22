<h1 id="b/5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Complete the square in the [augmented Lagrangian method](../../../../../augmented-lagrangian-method.md) objective:

$$
\boxed{\mathcal L_\mu(x,u)=f(x)+\frac1{2\mu}\|c(x)-\mu u\|_2^2-\frac\mu2\|u\|_2^2.}
$$

For fixed $u,\mu$, the last term is constant in $x$. Thus its minimization is the [quadratic penalty method](../../../../../quadratic-penalty-method.md) applied to the shifted constraint $c(x)=\mu u$.

Its practical advantage is that multiplier updates, typically $u^+=u-c(x)/\mu$, can drive the original constraint residual to zero while $\mu$ stays moderately sized. The plain [quadratic penalty method](../../../../../quadratic-penalty-method.md) generally needs $\mu$ very small to produce the same feasibility accuracy, exposing the conditioning problem in part (ii).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
