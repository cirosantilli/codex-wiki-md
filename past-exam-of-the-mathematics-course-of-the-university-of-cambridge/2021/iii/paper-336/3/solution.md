<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The linear $\cos x$ mode has frequency squared $k^2-1$, so $k_c(0)=1$. To resolve the small frequency near threshold, write

$$
k=1+\varepsilon^2\kappa+O(\varepsilon^4),
\qquad
T=\varepsilon t.
$$

The leading equation

$$
-\theta_{0,xx}-\theta_0=0
$$

and the initial data give

$$
\theta_0=A(T)\cos x,\qquad A(0)=1,\qquad A'(0)=0.
$$

At $O(\varepsilon^2)$, the equation for $\theta_2$ has a forcing whose $\cos x$ component is

$$
\frac34A^3-A''-2\kappa A.
$$

The [Fredholm solvability condition](../../../../../fredholm-solvability-condition.md) removes this [secular term](../../../../../secular-term.md) and yields the slow [amplitude equation](../../../../../amplitude-equation.md)

$$
\boxed{
A''+2\kappa A-\frac34A^3=0
}.
$$

It has the conserved energy

$$
E=\frac12(A')^2+\kappa A^2-\frac{3}{16}A^4.
$$

The potential has maxima at

$$
A^2=\frac{8\kappa}{3}.
$$

A periodic orbit launched from $A(0)=1$, $A'(0)=0$ exists only when that turning point lies inside the two maxima, namely

$$
\kappa>\frac38.
$$

At equality the orbit is the [separatrix](../../../../../separatrix.md); below it, the assumed real periodic oscillation is lost. Therefore

$$
\boxed{
k_c(\varepsilon)
=1+\frac38\varepsilon^2+O(\varepsilon^4)
}.
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 336](../../paper-336-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
