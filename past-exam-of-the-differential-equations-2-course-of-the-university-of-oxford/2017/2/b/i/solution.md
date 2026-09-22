<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The useful [change of independent variable in a second-order ODE](../../../../../change-of-independent-variable-in-a-second-order-ode.md) is $t=\log x$, followed by $y(x)=xv(t)$. The [chain rule](../../../../../chain-rule.md) gives

$$
y'=v+v_t,\qquad y''=x^{-1}(v_t+v_{tt}),\qquad Ly=xv_{tt}.
$$

Thus the [eigenvalue](../../../../../eigenvalue.md) equation becomes $v_{tt}=\lambda v$ on $0<t<1$, and the endpoint values become $v(0)=v(1)=0$. At the specified [eigenvalues](../../../../../eigenvalue.md),

$$
v(t)=A\cos(k\pi t)+B\sin(k\pi t).
$$

The first endpoint forces $A=0$; the second holds for every positive integer $k$. Choosing a convenient normalization yields

$$
\boxed{y_k(x)=x\sin(k\pi\log x),\qquad k=1,2,\ldots.}
$$

Each nonzero constant multiple is the same [eigenfunction](../../../../../eigenfunction.md) up to normalization. This [logarithmic conjugacy of a repeated-root Euler operator](../../../../../logarithmic-conjugacy-of-a-repeated-root-euler-operator.md) turns the [Cauchy-Euler equation](../../../../../cauchy-euler-equation.md) into the familiar [Fourier sine series](../../../../../fourier-sine-series.md) problem on a unit [interval](../../../../../interval-mathematics.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
