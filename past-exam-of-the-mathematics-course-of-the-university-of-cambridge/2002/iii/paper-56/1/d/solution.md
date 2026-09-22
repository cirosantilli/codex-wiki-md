<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The relevant [saddle equilibrium](../../../../../../saddle-equilibrium.md) is the origin, with [eigenvalues](../../../../../../eigenvalue.md)

$$
m_\pm=\frac{\kappa\pm\sqrt{\kappa^2-4\lambda}}2.
$$

For $\lambda<0$, they have opposite signs. Its [saddle index](../../../../../../saddle-index.md) is

$$
\boxed{\delta=-\frac{m_-}{m_+}
=\frac{\sqrt{\kappa^2-4\lambda}-\kappa}{\sqrt{\kappa^2-4\lambda}+\kappa}<1}
$$

near the homoclinic curve, because that curve has $\kappa>0$. Along its leading asymptote, $\delta=1-\tfrac45\sqrt{-\lambda}+o(\sqrt{-\lambda})$.

A local passage near the [saddle equilibrium](../../../../../../saddle-equilibrium.md) contributes a power $s^\delta$ to the [return map](../../../../../../poincare-map.md). Because $\delta<1$, its [derivative](../../../../../../derivative.md) becomes large as the orbit approaches the [separatrix](../../../../../../separatrix.md). The [periodic orbits](../../../../../../periodic-orbit.md) meeting the loops are therefore unstable, and their periods diverge logarithmically. On the side between the homoclinic and subcritical Hopf curves there are two unstable single-well [periodic orbits](../../../../../../periodic-orbit.md), surrounding the two [sink equilibria](../../../../../../sink-equilibrium.md). On crossing the double-loop curve downward, they join into one unstable outer [periodic orbit](../../../../../../periodic-orbit.md) surrounding both wells. The attracting outer [periodic orbit](../../../../../../periodic-orbit.md) is not the one that collides with the [saddle equilibrium](../../../../../../saddle-equilibrium.md): it persists across this global event.

The unstable outer [periodic orbit](../../../../../../periodic-orbit.md) must subsequently meet that attracting outer [periodic orbit](../../../../../../periodic-orbit.md) in a fold of [periodic orbits](../../../../../../periodic-orbit.md). This extra curve is required to obtain the six-region diagram. One can see its position from the same energy-balance calculation. After normalizing $a_0=1$, an outer Hamiltonian contour with $H>0$ selects

$$
\beta=B(H)=\frac{\int_0^{u_{\max}}u^2\sqrt{2H+u^2-u^4/2}\,du}
{\int_0^{u_{\max}}\sqrt{2H+u^2-u^4/2}\,du},
\qquad u_{\max}^2=1+\sqrt{1+4H}.
$$

At $H=0$, $B=4/5$. The [derivative](../../../../../../derivative.md) of the denominator diverges positively there, while that of the numerator stays finite, so $B$ initially decreases. Rescaling at large $H$ gives $B(H)\propto\sqrt H$, so it eventually increases. At its minimum the stable and unstable selected [periodic orbits](../../../../../../periodic-orbit.md) meet. Thus the [outer-cycle fold in a weakly perturbed double-well oscillator](../../../../../../outer-cycle-fold-in-a-weakly-perturbed-double-well-oscillator.md) has $\kappa_{\rm fold}=c_f(-\lambda)+o(|\lambda|)$ with $0<c_f<4/5$; quadrature gives $c_f\simeq0.75226$. The decreasing portion of $B(H)$ selects the unstable [periodic orbit](../../../../../../periodic-orbit.md), and the increasing portion selects the stable one, since the [energy](../../../../../../energy.md) drift has sign $\beta-B(H)$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
