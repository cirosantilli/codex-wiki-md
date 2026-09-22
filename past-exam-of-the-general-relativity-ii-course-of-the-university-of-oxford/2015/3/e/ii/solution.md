<h1 id="3/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the expanding flat branch $a(t)=Ae^{H_\Lambda t}$, with $A>0$. A [radial null geodesic in FLRW spacetime](../../../../../radial-null-geodesic-in-flrw-spacetime.md) satisfies $d\rho/dt=\pm1/a(t)$. For the incoming [past light cone](../../../../../past-light-cone.md) of the [spacetime event](../../../../../event-relativity.md) $(t_0,\rho=0)$, integration gives

$$
\boxed{\rho(t;t_0)=\int_t^{t_0}\frac{ds}{a(s)}
=\frac1{H_\Lambda}\left(\frac1{a(t)}-\frac1{a(t_0)}\right),\qquad t\le t_0,}
$$

with arbitrary angular direction. Equivalently, [conformal time](../../../../../conformal-time.md) $\eta=-1/(H_\Lambda a)$ gives $\rho=\eta_0-\eta$.

Let the reception time tend to infinity. The largest [comoving radial distance](../../../../../comoving-radial-distance.md) from which a signal emitted at time $t$ can reach the central [comoving observer](../../../../../comoving-observer.md) is

$$
\rho_{\mathrm h}(t)=\int_t^\infty\frac{ds}{a(s)}=\frac1{H_\Lambda a(t)}.
$$

Thus the [cosmological event horizon](../../../../../cosmological-event-horizon.md) has constant [proper distance in cosmology](../../../../../proper-distance-in-cosmology.md):

$$
\boxed{\rho=\frac1{H_\Lambda a(t)},\qquad D_{\mathrm h}=a(t)\rho_{\mathrm h}=H_\Lambda^{-1}.}
$$

An emitted [spacetime event](../../../../../event-relativity.md) is seen at a finite time if and only if $a(t)\rho<H_\Lambda^{-1}$. Equality would require $t_0=\infty$, while an event with $a(t)\rho>H_\Lambda^{-1}$ never reaches the observer. This is a bound on events at their emission time; a fixed [comoving observer](../../../../../comoving-observer.md) can have earlier visible events and later invisible ones.

The boundary really is a [null hypersurface](../../../../../null-hypersurface.md). For $f(t,\rho)=\rho-[H_\Lambda a(t)]^{-1}$, its normal has components $\partial_tf=1/a$ and $\partial_\rho f=1$, so

$$
g^{\mu\nu}\partial_\mu f\partial_\nu f=-\frac1{a^2}+\frac1{a^2}=0.
$$

The finite future integral, and hence this [observer event horizon](../../../../../observer-event-horizon.md), uses the expanding branch. For the contracting flat solution $a=Ae^{-H_\Lambda t}$, the same integral diverges and there is no future [observer event horizon](../../../../../observer-event-horizon.md) of this kind; the static zero-density solution likewise has none.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the general relativity II course of the University of Oxford](../../../../split.md)
6. [General relativity II course of the University of Oxford](../../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
