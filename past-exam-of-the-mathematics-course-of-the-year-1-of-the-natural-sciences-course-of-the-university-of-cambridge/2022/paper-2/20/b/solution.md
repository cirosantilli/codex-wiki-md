<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $t>0$, differentiate the printed ansatz:

$$
h=a t^{-1/3}-\frac{ax^2}{t}-bt,\qquad
h_t=-\frac a3t^{-4/3}+\frac{ax^2}{t^2}-b,
$$



$$
h_x=-\frac{2ax}{t},\qquad
(hh_x)_x=6a^2\frac{x^2}{t^2}-2a^2t^{-4/3}+2ab.
$$

Matching the independent coefficients in $h_t=(hh_x)_x-1$ gives

$$
a=6a^2,\qquad \frac a3=2a^2,\qquad b(1+2a)=1.
$$

There are two parameter pairs, including the degenerate spatially constant case:

$$
\boxed{(a,b)=\left(\frac16,\frac34\right)\quad\text{or}\quad(a,b)=(0,1)}.
$$

Their corresponding solutions are

$$
\boxed{h(x,t)=\frac1{6t^{1/3}}-\frac{x^2}{6t}-\frac34t}
\qquad\text{and}\qquad
\boxed{h(x,t)=-t}.
$$

The request for “the general form” cannot mean the complete solution set of this nonlinear [partial differential equation](../../../../../partial-differential-equation-split.md): substitution of one ansatz cannot provide arbitrary initial data, and the [superposition principle](../../../../../superposition-principle.md) does not apply.

A useful wider family follows by allowing an independent time-dependent constant term and quadratic coefficient, $h=A(t)+B(t)x^2$. Coefficient comparison gives $B'=6B^2$ and $A'=2AB-1$. For $B\ne0$, write $\tau=t-t_0>0$ to obtain $B=-1/(6\tau)$ and $A=C\tau^{-1/3}-3\tau/4$. Spatial translation, also a symmetry of the equation, therefore gives

$$
\boxed{h(x,t)=C\tau^{-1/3}-\frac{(x-x_0)^2}{6\tau}-\frac34\tau,
\qquad\tau=t-t_0>0}.
$$

Here $C,x_0,t_0$ are arbitrary constants; the displayed nontrivial ansatz corresponds to $C=1/6$ and $x_0=t_0=0$. There are also affine solutions $h=px+(p^2-1)t+q$, including the spatially constant branch. These are valid solution families, rather than a claim of a full general solution.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
