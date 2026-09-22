<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

For the [angularly resolved molecular arrival flux](../../../../../angularly-resolved-molecular-arrival-flux.md), let $f(v)$ be normalized by $\int_0^\infty f(v)\,dv=1$. Isotropic velocity directions have probability $d\Omega/(4\pi)$. Integrating over azimuth gives $(1/2)\sin\theta\,d\theta$, while the speed normal to a stationary piston is $v\cos\theta$. For incident directions $0\leq\theta\leq\pi/2$, the arrival flux is therefore

$$
\boxed{d\Gamma=\frac12nf(v)v\cos\theta\sin\theta\,d\theta\,dv.}
$$

An elastic collision transfers normal momentum $2mv\cos\theta$ to the piston. Integrating the momentum flux gives

$$
p=nm\int_0^\infty v^2f(v)\,dv\int_0^{\pi/2}\cos^2\theta\sin\theta\,d\theta=\boxed{\frac13nm\langle v^2\rangle}.
$$

No specific Maxwellian speed distribution was needed for this isotropic kinetic-[pressure](../../../../../pressure-split.md) identity.

Use the figure's $+x$ direction toward the piston and let its inward speed $u>0$ mean piston velocity $-u\hat{\mathbf x}$. For [reflection from a translating planar piston](../../../../../reflection-from-a-translating-planar-piston.md), in the piston frame the incoming normal velocity is $v_x+u$. Elastic reflection reverses it, and transforming back gives

$$
\boxed{(v_x,v_y,v_z)\longmapsto(-v_x-2u,v_y,v_z).}
$$

The exact kinetic-energy change in this ideal massive-piston model is $\Delta K=2muv_x+2mu^2$. Thus, to first order in the small piston speed,

$$
\boxed{K_{\rm after}=K_{\rm before}+2muv_x+O(u^2).}
$$

The [first-order collision-flux approximation for a slow piston](../../../../../first-order-collision-flux-approximation-for-a-slow-piston.md) applies: the incident collision flux changes at order $u$, but its product with the order-$u$ energy increment changes the energy rate only at order $u^2$. Hence one may use the stationary flux at leading order. For piston area $S$,

$$
\frac{dU}{dt}=S\int(2muv\cos\theta)\,d\Gamma=\frac13Snmu\langle v^2\rangle=\boxed{pSu=-p\frac{dV}{dt}.}
$$

Here $dV/dt=-Su$. This [compression work from molecular impacts](../../../../../compression-work-from-molecular-impacts.md), with no [heat](../../../../../heat-split.md) flow, is the first law for work done on the gas by compression. The derivation assumes $u$ small compared with thermal speeds and an approximately isotropic distribution at the piston; rapid compression can produce nonequilibrium [pressure](../../../../../pressure-split.md) and higher-order corrections.

## ↑ Ancestors (14)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
