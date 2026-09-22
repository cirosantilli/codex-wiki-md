<h1 id="37c/solution">Solution</h1>

↑ **Parent:** [37C](../37c.md)

The acoustic pressure satisfies $p_{tt}=c_0^2\Delta p$. Rigid walls impose vanishing normal velocity, equivalently the [Neumann boundary condition](../../../../../neumann-boundary-condition.md) on pressure. Separation of variables gives transverse modes $\cos(m\pi x/a)\cos(n\pi y/a)$ with $m,n\ge0$. With axial factor $e^{ikz-i\omega t}$, their [dispersion relation](../../../../../dispersion-relation.md) is

$$
\boxed{\omega^2=c_0^2\left[k^2+\frac{\pi^2}{a^2}(m^2+n^2)\right].}
$$

The $(0,0)$ mode is nondispersive. Every other mode propagates only above its [waveguide cutoff frequency](../../../../../waveguide-cutoff-frequency.md) $\omega_{mn}=\pi c_0\sqrt{m^2+n^2}/a$. Thus $\omega_{\min}=\pi c_0/a$.

Expand the prescribed entrance pressure in this cosine basis, with coefficients $A_{mn}$. Impose outgoing propagation and decay at infinity, with no incoming disturbance. At $\omega=\omega_{\min}/2$, only the constant transverse mode propagates, with $k_{00}=\pi/(2a)$. All other modes have $k=i\chi_{mn}$, where $\chi_{mn}=\pi\sqrt{m^2+n^2-1/4}/a$. The exact modal field is the outgoing constant mode plus $\sum_{m+n>0}A_{mn}\cos(m\pi x/a)\cos(n\pi y/a)e^{-\chi_{mn}z-i\omega t}$.

Since the slowest evanescent decay rate is $\sqrt3\pi/(2a)$, the far field is

$$
\boxed{\widetilde p(x,y,z,t)\sim\left[\frac1{a^2}\int_0^a\int_0^a\widetilde P(x,y)\,dx\,dy\right]e^{i\pi z/(2a)-i\omega t},\qquad z\gg a.}
$$

If that area average is zero, there is no propagating far-field component, and the field decays exponentially instead. For sufficiently regular entrance data the omitted terms are $O(e^{-\sqrt3\pi z/(2a)})$.

## ↑ Ancestors (10)

1. [37C](../37c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
