<h1 id="a/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $y=e^{S/\delta}$ and divide the equation by $y$:

$$
\frac{\epsilon}{\delta^2}(S')^2+
\frac{\epsilon}{\delta}S''+
\frac1\delta S'+x=0.
$$

Balancing the first and third terms gives $\delta=\epsilon$. With $S=S_0+\epsilon S_1+\cdots$, the terms of order $\epsilon^{-1}$ and one give

$$
S_0'(S_0'+1)=0,\qquad
(2S_0'+1)S_1'+S_0''+x=0.
$$

For the slow branch $S_0'=0$, choose $S_0=0$ and obtain $S_1=-x^2/2$. For the fast branch $S_0'=-1$, choose $S_0=-x$ and obtain $S_1=x^2/2$. Additive integration constants enter the two independent amplitudes. The two-term [WKB approximation](../../../../../wkb-approximation.md) is consequently

$$
y(x)\approx A e^{-x^2/2}+B e^{-x/\epsilon+x^2/2}.
$$

Imposing the [boundary conditions](../../../../../boundary-condition.md) on these two approximating modes yields

$$
\boxed{
y(x)\approx
\frac{e^{-x^2/2}-e^{-x/\epsilon+x^2/2}}
{e^{-1/2}-e^{-1/\epsilon+1/2}}.}
$$

This uses the first two exponent [functions](../../../../../function-split.md) $S_0,S_1$ for both branches. The next transport equations, if desired to identify the algebraic error, give $S_2=x-x^3/3$ for the slow mode and $S_2=x+x^3/3$ for the fast mode. Thus each displayed mode has relative amplitude correction $1+O(\epsilon)$ uniformly on the fixed interval; no [turning point](../../../../../turning-point.md) occurs because the two leading exponent roots remain distinct.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
