<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

Periodic boundary conditions give wavevectors $\mathbf k=(2\pi/L)(n_1,n_2)$. Each state occupies area $(2\pi/L)^2$ in wavevector space. A ring of radius $k$ contains $L^2(2\pi k\,dk)/(2\pi)^2$ states. With $\epsilon=\hbar^2k^2/(2m)$, $k\,dk=m\,d\epsilon/\hbar^2$, giving

$$
\boxed{g(\epsilon)=\frac{L^2m}{2\pi\hbar^2}\quad(\epsilon>0).}
$$

There is no spin degeneracy. At temperature $T>0$, set $z=e^{\mu/(k_BT)}<1$. The Bose occupation integral gives

$$
\frac N{L^2}=\frac{m}{2\pi\hbar^2}\int_0^\infty\frac{d\epsilon}{z^{-1}e^{\epsilon/(k_BT)}-1}
=\boxed{-\frac{mk_BT}{2\pi\hbar^2}\log(1-z).}
$$

The integral follows by expanding the denominator as $\sum_{\ell\geq1}z^\ell e^{-\ell\epsilon/(k_BT)}$ and integrating each positive term.

As $\mu\uparrow0$, this density diverges. Thus the excited states never have a finite maximum capacity at a positive temperature: every finite prescribed density can be accommodated with a strictly negative [chemical potential](../../../../../chemical-potential.md). The ground-state occupation then stays finite as area tends to infinity and its fraction vanishes. Hence **there is no [Bose-Einstein condensation](../../../../../bose-einstein-condensation.md) at any positive temperature in this homogeneous ideal two-dimensional gas**. At exactly zero temperature the [ground state](../../../../../ground-state.md) is occupied; the printed phrase about any temperature is understood as absence of a nonzero critical temperature, not exclusion of that zero-temperature limit.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
