<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Fourier transform](../../../../../fourier-transform-split.md) convention $\widehat u(s,t)=\int_{\mathbb R}e^{-isx}u(x,t)\,dx$. Then $\widehat{u_{xx}}=-s^2\widehat u$ and $\widehat{xu}=i\partial_s\widehat u$, so

$$
\widehat{\partial_x(xu)}=is(i\partial_s\widehat u)=-s\partial_s\widehat u.
$$

Thus the transformed [partial differential equation](../../../../../partial-differential-equation-split.md) and [initial condition](../../../../../initial-condition.md) are

$$
\boxed{\partial_t\widehat u+s\partial_s\widehat u=-s^2\widehat u,\qquad\widehat u(s,0)=1.}
$$

The last equality is the [Fourier transform](../../../../../fourier-transform-split.md) of the [Dirac delta distribution](../../../../../dirac-delta-function.md). The two terms in $\partial_x(xu)=u+xu_x$ must be transformed together; dropping $u$ would give the wrong equation.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
