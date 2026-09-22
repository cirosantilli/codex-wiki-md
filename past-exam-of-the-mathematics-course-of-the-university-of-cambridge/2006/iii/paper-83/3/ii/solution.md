<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a continuous size distribution, let $c_0(w)\,dw$ be initial [particle volume fraction](../../../../../../particle-volume-fraction.md) in a settling-speed interval. The [settling exposure for a particle size distribution](../../../../../../settling-exposure-for-a-particle-size-distribution.md) gives

$$
c(w,t)=c_0(w)e^{-wJ(t)},\qquad
g'(J)=\int_0^\infty b(w)c_0(w)e^{-wJ}\,dw.
$$

The spectrum continually shifts toward slower-settling particles. The deposit becomes progressively finer outward, with a smooth range of depositional distances instead of two distinct size components. Size-resolved deposition is $\rho_p(w)w\int_{t_a(r)}^\infty c_0(w)e^{-wJ(t)}dt$ per speed interval.

There is no universal monodisperse runout formula with an arbitrarily chosen mean settling speed. The box relation is

$$
R^4-R_0^4=4\mathsf F(\mathcal V/\pi)^{3/2}\int_0^J\sqrt{g'(s)}\,ds.
$$

A spectrum bounded away from zero settling speed has a finite limiting radius, but an arbitrarily slow-settling tail can extend the reach substantially or remove a finite runout bound. For example, if $b(w)c_0(w)\sim Cw^p$ near $w=0$, $p>-1$, its [Laplace transform](../../../../../../laplace-transform.md) behaves as $g'(J)\sim C\Gamma(p+1)J^{-(p+1)}$. The runout [integral](../../../../../../integral.md) converges only for $p>1$. A positive population with exactly zero settling speed retains [buoyancy](../../../../../../buoyancy.md) indefinitely and spreads without a finite radius limit in this no-entrainment model. Thus the fine tail of the actual distribution, and possible lofting when thermal [buoyancy](../../../../../../buoyancy.md) is restored, control the distal outcome.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
