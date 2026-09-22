<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Seek a [Frobenius series](../../../../frobenius-solution.md) $y=x^r\sum_{n\geq0}a_nx^n$, with $a_0\ne0$, on the positive side of zero. The lowest [coefficient](../../../../coefficient.md) gives the [indicial equation](../../../../indicial-equation.md) from part (a); the next gives $(r+1)(2r-1)a_1=0$. For either permitted [indicial exponent](../../../../indicial-exponent.md), $a_1=0$. Matching the subsequent powers gives

$$
a_{n+2}=-\frac{n+r+\lambda}{(n+r+2)(2n+2r+1)}a_n,\qquad n\geq0.
$$

The two [indicial exponents](../../../../indicial-exponent.md) differ by a noninteger, so there are two independent Frobenius solutions without a logarithmic companion. Normalizing each leading [coefficient](../../../../coefficient.md) to one, their forms are

$$
f_0(x)=1-\frac\lambda2x^2+O(x^4),\qquad
f_{3/2}(x)=x^{3/2}\left[1-\frac{2\lambda+3}{28}x^2+O(x^4)\right].
$$

Thus the general local solution is $C_0f_0+C_1f_{3/2}$. The endpoint condition at zero forces $C_0=0$. For a nontrivial solution, $C_1\ne0$, so $y(x)\sim C_1x^{3/2}$ and **$\alpha=3/2$**, with the arbitrary nonzero amplitude understood.

The condition at one selects values of $\lambda$ for which this branch also vanishes there; it does not change the selected local exponent. The zero solution, available for every $\lambda$, has no nonzero leading [coefficient](../../../../coefficient.md) and is excluded when asking for a leading exponent. This is a direct application of the [Frobenius method](../../../../frobenius-method.md) and the noninteger-separated-root case.[§2.7(i), equations 2.7.3–2.7.4](../../../../nist-digital-library-of-mathematical-functions.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
