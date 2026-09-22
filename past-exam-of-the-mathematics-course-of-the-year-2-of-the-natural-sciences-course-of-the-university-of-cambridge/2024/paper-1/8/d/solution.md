<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At zero the [indicial equation](../../../../../indicial-equation.md) is $\nu(\nu-1)+\nu=\nu^2=0$, with repeated [indicial root](../../../../../indicial-root.md) zero. To exhibit the analytic solution rather than only its candidate exponent, clear the denominator in the normal form:

$$
x(x-m)^2y''+(2x-m)(x-m)y'+\omega^2x^3y=0.
$$

Substitute $y_1=\sum_{n\geq0}b_nx^n$ and equate coefficients. With $b_j=0$ for negative indices, the [linear recurrence relation](../../../../../linear-recurrence-relation.md) is

$$
\boxed{m^2(n+1)^2b_{n+1}=mn(2n+1)b_n-n(n-1)b_{n-1}-\omega^2b_{n-3},\qquad n\geq0.}
$$

Every leading coefficient on the left is nonzero. Hence $b_0\ne0$ is free and all later coefficients are determined; the [Frobenius method](../../../../../frobenius-method.md) guarantees local convergence up to the next singularity. In particular,

$$
b_1=b_2=b_3=0,\qquad b_4=-\frac{\omega^2b_0}{16m^2},\qquad y_1=b_0\left[1-\frac{\omega^2x^4}{16m^2}+O(x^5)\right].
$$

For a second solution, use [reduction of order](../../../../../reduction-of-order.md). Writing $y_2=y_1v$ gives $W=y_1^2v'$, so part (c) yields

$$
\boxed{y_2(x)=y_1(x)\int^x\frac{C\,ds}{s(s-m)y_1(s)^2},\qquad C\ne0.}
$$

The additive constant in the [integral](../../../../../integral-split.md) only adds a multiple of $y_1$. As $x\downarrow0$ within $(0,m)$, its integrand is

$$
\frac{C}{x(x-m)y_1(x)^2}=-\frac{C}{mb_0^2}\frac1x+O(1).
$$

Therefore

$$
\boxed{y_2(x)=c_0\log x+O(1),\qquad c_0=-\frac{C}{mb_0}\ne0.}
$$

The nonzero [Wronskian](../../../../../wronskian.md) proves [linear independence](../../../../../linear-independence.md), and the logarithm is unavoidable for this second local solution.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
