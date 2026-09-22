<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [matter density parameter](../../../../matter-density-parameter.md) at general [scale factor](../../../../scale-factor-cosmology.md) is

$$
\Omega_m(a)=\frac{\Omega a^{-3}}{\Omega a^{-3}+(1-\Omega)a^{-2}}=\frac1{1+x}.
$$

The reference to the definition of $x$ in the printed part points to the wrong equation number: the needed definition is the substitution in part (b). Write $B=(1-\Omega)/\Omega$, so $x=Ba$, $d/da=B\,d/dx$, and

$$
H=\frac{H_0(1-\Omega)^{3/2}}{\Omega}\,x^{-3/2}(1+x)^{1/2}.
$$

Expanding the [matter growth equation as a function of scale factor](../../../../matter-growth-equation-as-a-function-of-scale-factor.md) first gives

$$
\frac{d^2\delta}{da^2}+\left(\frac3a+\frac{d\ln H}{da}\right)\frac{d\delta}{da}-\frac{3\Omega_m(a)}{2a^2}\delta=0.
$$

Using $d\ln H/dx=-3/(2x)+1/[2(1+x)]$ and dividing by $B^2$, we obtain

$$
\boxed{\delta''+\frac12\left(\frac3x+\frac1{1+x}\right)\delta'-\frac{3\delta}{2x^2(1+x)}=0,}
$$

where these primes denote [derivatives](../../../../derivative.md) with respect to $x$. For the proposed [linear cosmological density perturbation](../../../../linear-cosmological-density-perturbation-split.md) $\delta_1=(1+x)^{1/2}x^{-3/2}$,

$$
\frac{\delta_1'}{\delta_1}=-\frac{2x+3}{2x(1+x)},\qquad
\frac{\delta_1''}{\delta_1}=\frac{8x^2+24x+15}{4x^2(1+x)^2}.
$$

The left side of the [differential equation](../../../../differential-equation-split.md), divided by $\delta_1$, has numerator

$$
(8x^2+24x+15)-(4x+3)(2x+3)-6(1+x)=0
$$

over the common denominator $4x^2(1+x)^2$. This proves the result directly. Also $\delta_1'/\delta_1<0$ for every $x>0$, so it is a **decaying mode**:

$$
\boxed{\delta_1\sim x^{-3/2}\quad(x\to0),\qquad \delta_1\sim x^{-1}\quad(x\to\infty).}
$$

It is proportional to the [Hubble parameter](../../../../hubble-parameter.md), an instance of the [Hubble parameter as a solution of the dust growth equation](../../../../hubble-parameter-as-a-solution-of-the-dust-growth-equation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the cosmology course of the University of Oxford](../../../split.md)
5. [Cosmology course of the University of Oxford](../../../../cosmology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
