<h1 id="32e/solution">Solution</h1>

↑ **Parent:** [32E](../32e.md)

Insert the finite exponential expansion into the [Gelfand-Levitan-Marchenko equation](../../../../../marchenko-equation.md). The integral contribution is

$$
\sum_{m,n}K_m(x)\beta_n e^{-c_ny}\frac{e^{-(c_m+c_n)x}}{c_m+c_n}.
$$

Comparing coefficients of $e^{-c_ny}$ gives

$$
\boxed{A_{nm}(x)=\delta_{nm}+\frac{\beta_n e^{-(c_n+c_m)x}}{c_n+c_m},\qquad B_n(x)=-\beta_n e^{-c_nx}}.
$$

For this coefficient comparison take the $c_n$ distinct; repeated exponents can first be combined. The linear system supplies the coefficients whenever its matrix is invertible.

In the [inverse scattering transform](../../../../../inverse-scattering-transform.md) convention $u_t-6uu_x+u_{xxx}=0$, the [Korteweg-De Vries equation](../../../../../korteweg-de-vries-equation.md) solution is $u=-2\,dK(x,x)/dx$. The reflectionless scattering data evolve as $\beta_n(t)=\beta_n(0)e^{8c_n^3t}$, with the $c_n$ fixed. For one exponential,

$$
K(x,y)=-\frac{\beta_1e^{-c(x+y)}}{1+(\beta_1/2c)e^{-2cx}}.
$$

Differentiating its diagonal gives

$$
\boxed{u(x,t)=-\frac{4\beta_1c e^{-2cx}}{(1+(\beta_1/2c)e^{-2cx})^2}}.
$$

For $\beta>0$, this is the smooth [soliton](../../../../../soliton.md)

$$
u=-2c^2\operatorname{sech}^2\!\left(cx-4c^3t-\tfrac12\log(\beta/(2c))\right).
$$

It travels at speed $4c^2$. If $\beta=0$ the solution is zero; if $\beta<0$ the denominator vanishes somewhere, so the formula is not a globally smooth one-soliton. Positivity is the necessary qualification for a regular soliton.

## ↑ Ancestors (10)

1. [32E](../32e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
