<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For real positive weight $w$, the [weighted inner product](../../../../weighted-inner-product.md) is

$$
\boxed{\langle y_1,y_2\rangle_w=\int_a^b y_1(x)^*y_2(x)w(x)\,dx.}
$$

The functions must have finite weighted norm; the conjugate is omitted for real functions. Multiplying the differential equation by $xe^{-x}$ gives

$$
(xe^{-x}y')'+ne^{-x}y=0.
$$

Thus the [Sturm-Liouville form](../../../../sturm-liouville-form.md) has $p=xe^{-x}$, $q=0$ and $w=e^{-x}$. With the positive-sign spectral convention define

$$
\boxed{\mathcal Ay=-\frac1w(py')'=-xy''+(x-1)y',\qquad\mathcal Ay=ny.}
$$

The existing [Laguerre differential operator on polynomials](../../../../laguerre-differential-operator-on-polynomials.md) uses the opposite operator $L=-\mathcal A$, with eigenvalues $-n$; keeping this sign convention explicit avoids confusing the two descriptions.

For admissible $f,g$, [integration by parts](../../../../integration-by-parts.md) gives

$$
\langle f,\mathcal Ag\rangle_w-\langle\mathcal Af,g\rangle_w=\left[xe^{-x}(f'^*g-f^*g')\right]_0^\infty.
$$

The boundary form must vanish for every pair in the self-adjoint domain. In the usual regular-at-zero Laguerre realization one imposes $\lim_{x\downarrow0}xe^{-x}y'=0$, excluding the logarithmic branch; at infinity one uses the weighted square-integrable domain with vanishing boundary form. A condition $y(\infty)=0$ would be inappropriate for polynomial eigenfunctions. For any pair of polynomials, the factor $x$ makes the boundary form zero at zero, while the exponential beats all polynomial growth at infinity. These functions also have finite weighted norms.

Self-adjointness yields $(n-m)\langle y_m,y_n\rangle_w=0$, giving [orthogonality of Sturm-Liouville eigenfunctions](../../../../orthogonality-of-sturm-liouville-eigenfunctions.md):

$$
\boxed{\int_0^\infty e^{-x}y_m(x)^*y_n(x)\,dx=0\quad(m\ne n).}
$$

For the specified polynomials, direct differentiation gives $\mathcal Au=u$ and $\mathcal Av=3v$. Hence their eigenvalues in the displayed convention are **1 and 3**, respectively, or **−1 and −3** for $L=-\mathcal A$.

To find the quadratic, put $h=ax^2+bx+c$. The equation $xh''+(1-x)h'+2h=0$ reduces to $(4a+b)x+(b+2c)=0$. Thus $b=-4a$, $c=2a$. Since $h(1)=-a=1$,

$$
\boxed{h(x)=-x^2+4x-2.}
$$

These are scalar multiples of the [Laguerre polynomials](../../../../laguerre-polynomial.md) of degrees one, three and two.

For $n=0$, the first integral is $xe^{-x}y'=C$, so all solutions with the prescribed interior normalization are

$$
y(x)=1+C\int_{x_0}^x\frac{e^t}{t}dt.
$$

Two independent choices are

$$
\boxed{y_1(x)=1,\qquad y_2(x)=1+\int_{x_0}^x\frac{e^t}{t}dt.}
$$

They both equal one at $x_0$, and their Wronskian is $e^x/x\ne0$. For sufficiently large $x$, the last unit interval contributes at least $e^{x-1}/x$, proving that $y_2\to\infty$. These are the [zero-eigenvalue solutions of the Laguerre differential equation](../../../../zero-eigenvalue-solutions-of-the-laguerre-differential-equation.md), with the second expressible through the [exponential integral](../../../../exponential-integral.md). It also has a logarithmic singularity at zero and is not an admissible polynomial or weighted square-integrable eigenfunction. An interior value alone does not enforce the endpoint conditions of the spectral problem.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2012](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
