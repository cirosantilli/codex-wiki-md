<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Convolution with the [retarded acoustic Green function](../../../../../../retarded-acoustic-green-function.md), followed by two integrations by parts in the source coordinate, yields

$$
\rho'(x,t)=\partial_{x_i}\partial_{x_j}\int\frac{T_{ij}(y,t-|x-y|/c_0)}{4\pi c_0^2|x-y|}\,dV_y.
$$

For the [acoustic compact-source approximation](../../../../../../acoustic-compact-source-approximation.md), replace the distance and the source [retarded time](../../../../../../retarded-time.md) by $r=|x|$ and $\tau=t-r/c_0$ in the leading moment. Thus the integral is $S_{ij}(\tau)/(4\pi c_0^2r)$, where $S_{ij}=\int T_{ij}\,dV$. In the [acoustic far field](../../../../../../acoustic-far-field.md), each spatial derivative acts predominantly on retarded time: $\partial_{x_i}\tau=-n_i/c_0$, where $n_i=x_i/r$. Derivatives of $1/r$ and of $n_i$ give lower powers of $r$. The two retarded derivatives therefore give

$$
\boxed{\rho'_Q(x,t)\sim\frac{n_i n_j\ddot S_{ij}(\tau)}{4\pi c_0^4r}
=\frac{x_i x_j\ddot S_{ij}(\tau)}{4\pi c_0^4r^3}}.
$$

This is the compact [acoustic quadrupole](../../../../../../acoustic-quadrupole.md) field, retaining its angular stress projection.

For the [compact acoustic quadrupole Mach-number scaling](../../../../../../compact-acoustic-quadrupole-mach-number-scaling.md), let the source length be $\ell$, typical fluctuation speed be $U$, and typical time be $\ell/U$. The low-[Mach number](../../../../../../mach-number.md) stress is $T=O(\rho_0U^2)$, so $S=O(\rho_0U^2\ell^3)$ and $\ddot S=O(\rho_0U^4\ell)$. Consequently

$$
\boxed{\rho'_Q/\rho_0=O\left(\frac{\ell}{r}m^4\right),\qquad m=U/c_0}.
$$

With the geometric ratio separated, this is the stated fourth-power dependence. It assumes an advective source time scale and compactness $\omega\ell/c_0=O(m)\ll1$. An externally driven source with an independent [frequency](../../../../../../frequency.md) does not acquire the same Mach power automatically.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
