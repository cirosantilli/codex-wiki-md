<h1 id="a/3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume first that $n\geq m$. Substituting [Rodrigues' formula](../../../../../rodrigues-formula.md) for $L_n$ gives

$$
I_{nm}=\frac1{n!}\int_0^\infty L_m(x)\frac{d^n}{dx^n}(x^ne^{-x})\,dx
=\frac{(-1)^n}{n!}\int_0^\infty L_m^{(n)}(x)x^ne^{-x}\,dx.
$$

Here [integration by parts](../../../../../integration-by-parts.md) was performed $n$ times. Each boundary term vanishes: at infinity a [polynomial](../../../../../polynomial-split.md) times $e^{-x}$ tends to zero; at zero every [derivative](../../../../../derivative.md) of $x^ne^{-x}$ of order less than $n$ vanishes. If $n>m$, the [derivative](../../../../../derivative.md) $L_m^{(n)}$ is zero, proving [orthogonality](../../../../../orthogonal-vectors.md). The case $m>n$ follows by exchanging the two factors.

For $m=n$, the leading coefficient found above gives $L_n^{(n)}=(-1)^n$. Therefore

$$
I_{nn}=\frac1{n!}\int_0^\infty x^ne^{-x}\,dx=\frac{\Gamma(n+1)}{n!}=1.
$$

The same conclusion includes $n=0$ directly. Thus the full [Laguerre orthonormality](../../../../../laguerre-orthonormality.md) relation is

$$
\boxed{\int_0^\infty L_n(x)L_m(x)e^{-x}\,dx=\delta_{nm}.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
