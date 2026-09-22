<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The plane separates the exterior into two half-domains. Use an [odd Legendre extension for an equatorial Dirichlet plane](../../../../../odd-legendre-extension-for-an-equatorial-dirichlet-plane.md) in each. On the upper hemisphere, extend $u+2u^2$ to the odd function $u+2u|u|$ on the whole sphere. On the lower hemisphere, the appropriate odd extension is $u-2u|u|$. Define, for odd $\ell$,

$$
b_\ell=2(2\ell+1)\int_0^1t^2P_\ell(t)\,dt.
$$

The [orthogonality](../../../../../orthogonal-vectors.md) and parity of the [Legendre polynomials](../../../../../legendre-polynomial.md) give the solution in both half-domains as

$$
\boxed{\Psi(r,\theta)=\frac{a^2}{r^2}u+\operatorname{sgn}(u)\sum_{\ell=1,3,5,\ldots}b_\ell\left(\frac ar\right)^{\ell+1}P_\ell(u),\quad u=\cos\theta.}
$$

Set its value on $u=0$ to zero. The first coefficients are $b_1=3/2$ and $b_3=7/12$. All odd [Legendre polynomials](../../../../../legendre-polynomial.md) vanish at zero, so the plane condition holds. On the sphere the sum is $2u|u|$, and multiplication by $\operatorname{sgn}(u)$ recovers $2u^2$ on either side. Thus the original sphere data and decay at infinity both hold. A jump of the normal [derivative](../../../../../derivative.md) at the sheet is permitted; the sheet can support induced [surface charge density](../../../../../surface-charge-density.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
