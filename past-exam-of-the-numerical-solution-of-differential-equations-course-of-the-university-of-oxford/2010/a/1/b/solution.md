<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [zero-stable](../../../../../zero-stability.md) has a uniformly bounded response to small perturbations of its starting values and accumulated residuals on a fixed time interval as $h\to0$. Equivalently, its first characteristic [polynomial](../../../../../polynomial-split.md) satisfies the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md): every [root](../../../../../root-of-a-root-system.md) has modulus at most one, and each [root](../../../../../root-of-a-root-system.md) on the unit circle is simple.

For the consistent parameters, the recurrence for $y'=0$ is $y_{n+3}-2y_{n+1}+y_n=0$, with characteristic [polynomial](../../../../../polynomial-split.md)

$$
\rho(z)=z^3-2z+1=(z-1)(z^2+z-1).
$$

Let $r=(-1-\sqrt5)/2$. Choose $y_1=r$ and $y_2=r^2$; together with $y_0=1$ these generate exactly $y_n=r^n$. Since $|r|=(1+\sqrt5)/2>3/2$,

$$
\boxed{|y_n|=\left(\frac{1+\sqrt5}{2}\right)^n\geq(3/2)^n.}
$$

This parasitic mode violates the [root](../../../../../root-of-a-root-system.md) condition and grows without a bound independent of the number of steps. Scaling its starting amplitudes gives the same unbounded amplification for arbitrarily small initial perturbations. Thus **the only consistent method in the family is not zero-stable**.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
