<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The original PDF supplies the intended profiles $\rho=\rho_1f(\eta)$, $p=\rho_1\dot R^2g(\eta)$ and $u=\dot Rh(\eta)$; the TeX has corrupted the first two. At fixed $r$, $\partial_t\eta=-\eta\dot R/R$, and at fixed $t$, $\partial_r\eta=1/R$. The spherical [continuity equation](../../../../../../../continuity-equation.md) is therefore

$$
0=\partial_t\rho+\frac1{r^2}\partial_r(r^2\rho u)=\frac{\rho_1\dot R}{R}\left[-\eta f'+\frac1{\eta^2}(\eta^2fh)'\right].
$$

Since $\dot R/R=3/(5t)$ is nonzero, the [continuity equation for a superbubble similarity solution](../../../../../../../continuity-equation-for-a-superbubble-similarity-solution.md) is

$$
\boxed{-\eta f'+\frac1{\eta^2}(\eta^2fh)'=0,\qquad\text{or}\qquad(h-\eta)f'+fh'+\frac{2fh}{\eta}=0.}
$$

The ambient gas is at rest. In the locally stationary [shock frame](../../../../../../../shock-frame.md), its velocity is $-\dot R$; the downstream velocity is $u-\dot R$. Using the [shock compression ratio](../../../../../../../shock-compression-ratio.md) from part (a) converts the downstream speed back to the laboratory frame and gives the inner shock boundary conditions

$$
\boxed{f(1^-)=\frac{\gamma+1}{\gamma-1},\qquad g(1^-)=\frac2{\gamma+1},\qquad h(1^-)=\frac2{\gamma+1}.}
$$

Immediately outside the shock, the corresponding unperturbed profiles are $f=1$, $g=0$ and $h=0$, with $g=0$ understood in the negligible-ambient-pressure limit.

The inner boundary must supply the injected power. If the source is idealized as a point and the profiles extend all the way inward, [central energy input in a similarity solution](../../../../../../../central-energy-input-in-a-similarity-solution.md) requires

$$
\lim_{r\downarrow0}4\pi r^2u\left(\frac{\rho u^2}{2}+\frac{\gamma p}{\gamma-1}\right)=\dot E,
$$

or equivalently $\lim_{\eta\downarrow0}\eta^2h(fh^2/2+\gamma g/(\gamma-1))=125/(108\pi\alpha^5)$. A finite source region or an inner wind/contact region supplies a different matching description. One cannot impose a regular zero-flux centre on a source-free interior and still inject nonzero power.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 314](../../../../paper-314-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
