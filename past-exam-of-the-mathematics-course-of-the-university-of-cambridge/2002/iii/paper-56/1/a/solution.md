<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) have $y=0$ and $x(\lambda+x^2)=0$. Thus

$$
\boxed{O=(0,0)\text{ for all parameters},\qquad P_\pm=(\pm\sqrt{-\lambda},0)\text{ for }\lambda<0.}
$$

At $O$, the [linearization](../../../../../../linearization.md) has [trace](../../../../../../matrix-trace.md) $\kappa$ and [determinant](../../../../../../determinant.md) $\lambda$. Hence $O$ is a [saddle equilibrium](../../../../../../saddle-equilibrium.md) when $\lambda<0$, a [sink equilibrium](../../../../../../sink-equilibrium.md) when $\lambda>0,\kappa<0$, and a [source equilibrium](../../../../../../source-equilibrium.md) when $\lambda>0,\kappa>0$. The [sink equilibrium](../../../../../../sink-equilibrium.md)/[source equilibrium](../../../../../../source-equilibrium.md) may be a [node equilibrium](../../../../../../node-dynamical-systems.md) or a [focus equilibrium](../../../../../../focus-dynamical-systems.md); the node-focus discriminant is not a [bifurcation](../../../../../../bifurcation.md) curve. At $P_\pm$, the [trace](../../../../../../matrix-trace.md) and [determinant](../../../../../../determinant.md) are $\kappa+\lambda$ and $-2\lambda$. These points are [sink equilibria](../../../../../../sink-equilibrium.md) for $\kappa<-\lambda$ and [source equilibria](../../../../../../source-equilibrium.md) for $\kappa>-\lambda$.

The local [bifurcation](../../../../../../bifurcation.md) curves are therefore

$$
\boxed{\lambda=0\quad\text{(pitchfork)},\qquad
\kappa=0,\ \lambda>0\quad\text{(Hopf at }O),\qquad
\kappa=-\lambda,\ \lambda<0\quad\text{(Hopf at }P_\pm).}
$$

For $\kappa\ne0$ on the pitchfork curve, a leading centre-manifold equation is $\dot x=(\lambda x+x^3)/\kappa+\cdots$. For $\kappa<0$, with unfolding parameter $-\lambda$, the pitchfork is supercritical and creates two [sink equilibria](../../../../../../sink-equilibrium.md) from a [sink equilibrium](../../../../../../sink-equilibrium.md) that becomes a [saddle equilibrium](../../../../../../saddle-equilibrium.md). For $\kappa>0$ it is subcritical in the centre direction; the nonzero branches are unstable, and the transverse [eigenvalue](../../../../../../eigenvalue.md) is also positive. The origin of parameter space is a reflection-symmetric double-zero degeneration.

To determine Hopf criticality at the origin, use the [energy](../../../../../../energy.md) $E=y^2/2+\lambda x^2/2+x^4/4$, whose [derivative](../../../../../../derivative.md) is $(\kappa-x^2)y^2$. For a small nearly harmonic oscillation $x=R\cos(\sqrt\lambda\,t)$, averaging gives $\dot R=\kappa R/2-R^3/8+\cdots$. Thus this [Hopf bifurcation](../../../../../../hopf-bifurcation.md) is supercritical and creates an attracting [periodic orbit](../../../../../../periodic-orbit.md) for $\kappa>0$. By the supplied opposite-criticality fact, the simultaneous [Hopf bifurcations](../../../../../../hopf-bifurcation.md) at the two nonzero [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) are subcritical. A direct calculation confirms this: writing $x=\sqrt{-\lambda}+X$, $Y=-y/\sqrt{-2\lambda}$ puts the cubic radial coefficient at $1/4>0$, including the contribution from the quadratic terms.

The figure includes these local curves and the global curves derived below. All lines emerging from the double-zero point are local asymptotic sketches.<a id="1/a/image-local-and-global-curves-near-the-symmetric-double-zero-point"></a>


![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-56-symmetric-parameters.png)

**[Figure 1](#1/a/image-local-and-global-curves-near-the-symmetric-double-zero-point). Local and global curves near the symmetric double-zero point**.

## ↑ Ancestors (11)

1. [A](../a.md)
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
