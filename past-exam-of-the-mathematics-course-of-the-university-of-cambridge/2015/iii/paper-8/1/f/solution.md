<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For the globally invertible [Hamiltonian flow](../../../../../../hamiltonian-flow.md) from (a), the general characteristic formula is

$$
f(t,z)=f_0(\Phi(0,t,z))+\int_0^t h(\Phi(s,t,z))\,ds.
$$

Every $\Phi(s,t)$ preserves [Lebesgue measure](../../../../../../lebesgue-measure.md), by (b). Thus composition with it is an [isometry](../../../../../../isometry.md) of each [Lp space](../../../../../../lp-space.md). The [Minkowski integral inequality](../../../../../../minkowski-integral-inequality.md) gives

$$
\boxed{\|f(t)\|_p\leq\|f_0\|_p+t\|h\|_p.}
$$

Applying the [Minkowski inequality](../../../../../../minkowski-inequality.md) also in time yields **the [finite-time Lp bound for Hamiltonian transport](../../../../../../finite-time-lp-bound-for-hamiltonian-transport.md)**:

$$
\boxed{\|f\|_{L^p([0,T]\times\mathbb R^{2d})}
\leq T^{1/p}\|f_0\|_p+
\left(\frac{T^{p+1}}{p+1}\right)^{1/p}\|h\|_p<\infty.}
$$

The smoothness assumptions allow the characteristic construction; the norm estimate itself only uses the [Lp space](../../../../../../lp-space.md) data and volume preservation.

For a concrete failure on infinite time, choose $\omega=1$, $f_0=0$, and

$$
h(x,v)=e^{-(|x|^2+|v|^2)/2}=e^{-H_1(x,v)}.
$$

This is smooth, time independent and in every finite [Lp space](../../../../../../lp-space.md); it is invariant under the [isotropic harmonic oscillator flow](../../../../../../isotropic-harmonic-oscillator-flow.md). Therefore **the solution grows linearly**:

$$
\boxed{f(t,x,v)=t\,h(x,v),\qquad
\int_0^\infty\|f(t)\|_p^p\,dt
=\|h\|_p^p\int_0^\infty t^p\,dt=\infty.}
$$

This [invariant-source secular growth in Hamiltonian transport](../../../../../../invariant-source-secular-growth-in-hamiltonian-transport.md) supplies the counterexample even with zero initial data.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
