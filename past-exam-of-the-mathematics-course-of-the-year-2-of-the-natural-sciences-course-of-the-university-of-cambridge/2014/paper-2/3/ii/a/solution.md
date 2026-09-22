<h1 id="3/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Impose a homogeneous [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) on the Green function in its first variable, $G(r,r')=0$ for $r\in S$. The second boundary term then vanishes, giving

$$
\boxed{\phi(r')=\int_S\phi(r)\partial_{n_r}G(r,r')\,dS.}
$$

In a bounded domain, a Dirichlet Green function requires $k^2$ not to be a Dirichlet eigenvalue of $-\Delta$; otherwise a resonance can obstruct its existence. The representation assumes such a Green function exists.

In all space, put $\rho=|r-r'|$ and try $G=Ae^{ik\rho}/\rho$. For $\rho>0$, direct differentiation gives $(\rho^2G')'+k^2\rho^2G=0$, so the [Helmholtz equation](../../../../../../helmholtz-equation.md) holds away from the source. Integrate its inhomogeneous version over a small source-centred ball. The $k^2G$ volume integral tends to zero, while the flux is

$$
\lim_{\varepsilon\downarrow0}4\pi\varepsilon^2G'(\varepsilon)=-4\pi A.
$$

It must equal the integrated delta, one. Therefore

$$
\boxed{A=-\frac1{4\pi},\qquad G(r,r')=-\frac{e^{ik|r-r'|}}{4\pi|r-r'|}.}
$$

This is the negative of the convention used in the [outgoing Green function for the three-dimensional Helmholtz equation](../../../../../../outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md), where the source is $-\delta$. The sign here follows the present $+\delta$ convention. The factor $e^{ik\rho}$ chooses the outgoing solution, with time convention $e^{-i\omega t}$ and the [Sommerfeld radiation condition](../../../../../../sommerfeld-radiation-condition.md); one could add homogeneous solutions without a radiation prescription.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [Ii](../../ii.md)
3. [3](../../../3.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
