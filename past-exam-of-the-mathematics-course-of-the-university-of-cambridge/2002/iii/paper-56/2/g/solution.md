<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The change of time is $d\tau/dt=u$, which is positive in the half-plane under consideration. Dividing the two approximate equations by $u$ gives

$$
\frac{du}{d\tau}=\mu+u-v,\qquad \frac{dv}{d\tau}=\lambda u.
$$

Set $w=v-\mu$. The inhomogeneous system becomes $(u,w)'=(u-w,\lambda u)$, with [eigenvalues](../../../../../../eigenvalue.md) $(1\pm\sqrt{1-4\lambda})/2$. For $\lambda>1/4$, write $\omega=\sqrt{4\lambda-1}/2$. Integrating with the prescribed initial data gives

$$
\boxed{u(\tau)=e^{\tau/2}\left[h\cos(\omega\tau)+\frac{\mu+h/2-v_0}{\omega}\sin(\omega\tau)\right],}
$$

and

$$
\boxed{v(\tau)=\mu+e^{\tau/2}\left[(v_0-\mu)\cos(\omega\tau)+
\frac{\lambda h-(v_0-\mu)/2}{\omega}\sin(\omega\tau)\right].}
$$

These expressions also verify both initial values and their initial [derivatives](../../../../../../derivative.md). For fixed $\mu>0$ and small $h,v_0$ on the outgoing branch, the sine coefficient in $u$ is positive and dominates the initial cosine term. The first return to small $u$ is near the first positive zero, $\omega\tau\simeq\pi$. Hence

$$
\boxed{\tau_{\rm excursion}\simeq\frac{\pi}{\omega}=\frac{2\pi}{\sqrt{4\lambda-1}}.}
$$

The factor is a half-turn of the growing spiral, not its full rotation period. After this excursion the approximate trajectory approaches the small-$u$, large-$v$ region. In the full system the term $-\lambda v$, omitted during the large excursion, allows the motion to descend along that region and return.

As $\lambda\downarrow1/4$, the rescaled excursion time diverges and the factor $e^{\tau/2}$ produces arbitrarily large excursions. At the critical value the matrix is a nontrivial Jordan block, and the limiting formula is

$$
u(\tau)=e^{\tau/2}[h+(\mu+h/2-v_0)\tau].
$$

For the small outgoing initial data this is positive and unbounded: the [unstable manifold](../../../../../../unstable-manifold.md) no longer turns back. Below $1/4$ the two [eigenvalues](../../../../../../eigenvalue.md) are real and positive, so there is again no oscillatory return. This [quadratic escape desingularization](../../../../../../quadratic-escape-desingularization.md) explains **loss of the [periodic orbit](../../../../../../periodic-orbit.md) at infinity**, together with the unstable-manifold escape, as $\lambda$ decreases through $1/4$. It is not a finite homoclinic [bifurcation](../../../../../../bifurcation.md) to the origin. The divergent $\tau$ travel time must not be identified with the physical period without integrating $dt=d\tau/u$; the time change becomes singular near $u=0$.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
