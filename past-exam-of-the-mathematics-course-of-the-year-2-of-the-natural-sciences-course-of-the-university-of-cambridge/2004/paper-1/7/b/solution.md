<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Divide the equation by $\sqrt{1-x^2}$ to obtain its [Sturm-Liouville form](../../../../../sturm-liouville-form.md):

$$
\boxed{\frac d{dx}\left(\sqrt{1-x^2}\,y'\right)+\frac{n^2}{\sqrt{1-x^2}}y=0.}
$$

Thus $p=\sqrt{1-x^2}$, $q=0$ and $w=(1-x^2)^{-1/2}$. For $L=-w^{-1}(p\,d/dx)'$, the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md) gives the endpoint form $[p(\bar f'g-\bar f g')]_{-1}^1$. A natural self-adjoint choice is

$$
\boxed{\lim_{x\to-1^+}\sqrt{1-x^2}\,y'(x)=\lim_{x\to1^-}\sqrt{1-x^2}\,y'(x)=0.}
$$

Under $x=\cos\theta$, these become the ordinary zero-derivative conditions at $\theta=0,\pi$ for $-d^2/d\theta^2$. They therefore define the realization whose [Neumann eigenfunctions of the Chebyshev differential operator](../../../../../neumann-eigenfunctions-of-the-chebyshev-differential-operator.md) are $T_n(x)=\cos(n\arccos x)$, with $n=0,1,\ldots$.

Boundedness alone does not choose these endpoint conditions: $\sin(n\arccos x)$ is also bounded but generally has a nonzero endpoint value of $py'$. Requiring bounded $y'$ is a sufficient stronger regularity condition for the displayed zero-flux limits. Other self-adjoint endpoint choices are possible; the boundary form and the operator domain must specify which is intended.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
