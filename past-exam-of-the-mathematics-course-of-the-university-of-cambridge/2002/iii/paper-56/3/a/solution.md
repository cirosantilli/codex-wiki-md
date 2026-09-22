<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A global [bifurcation](../../../../../../bifurcation.md) joins two mechanisms: a long passage near a [hyperbolic equilibrium point](../../../../../../hyperbolic-equilibrium-point.md) and a finite excursion returning the [unstable manifold](../../../../../../unstable-manifold.md) to its neighborhood. [Eigenvalue](../../../../../../eigenvalue.md) ratios control the local passage, while the geometry of the global return decides reinjection, folding and trapping. In the real symmetric case there are two returning branches and a power-law cusp. In the [saddle-focus](../../../../../../saddle-focus-equilibrium.md) case rotation adds infinitely many oscillations to that cusp. The following maps display both mechanisms explicitly.

For the Lorenz configuration, enter on $z=h$ at $(x,y,h)$ and leave on $x=s h$, where $s=\operatorname{sgn}(x)$. Solving the linear [flow](../../../../../../flow.md) gives a flight time

$$
T=\frac1{\lambda_+}\log\frac h{|x|}.
$$

Put $\gamma=-\widehat\lambda/\lambda_+>\delta=-\lambda_-/\lambda_+$. The outgoing coordinates are

$$
x_{\rm out}=s h,\qquad
y_{\rm out}=y(|x|/h)^\gamma,\qquad
z_{\rm out}=h(|x|/h)^\delta.
$$

The smooth global map from each outgoing section to the incoming section has, to leading order,

$$
x_{\rm new}=s[-\mu+a z_{\rm out}]+O(y_{\rm out},z_{\rm out}^2),\qquad
y_{\rm new}=s\nu+O(z_{\rm out},y_{\rm out}),
$$

up to the choice of which unstable branch carries the sign of $\nu$. Reflection [symmetry](../../../../../../symmetry-physics.md) makes the offsets opposite and the leading coefficients equal. Since the stable transverse coordinate is multiplied by the higher power $|x|^\gamma$, it contributes only subleading terms to the leading scalar map. Absorbing powers of $h$ into a positive constant gives the [Lorenz power return map](../../../../../../lorenz-power-return-map.md)

$$
\boxed{x_{\rm new}=f_L(x)=\operatorname{sgn}(x)(-\mu+A|x|^\delta).}
$$

The line $x=0$ lies on the [stable manifold](../../../../../../stable-manifold.md) and has no finite return; the discontinuity is therefore a genuine missing return, not an arbitrary value to assign at zero.

If $\delta>1$, the [derivative](../../../../../../derivative.md) $A\delta|x|^{\delta-1}$ tends to zero. For $\mu<0$, there are two attracting [fixed points](../../../../../../fixed-point.md), $x=\pm s$ with $s=-\mu+As^\delta\simeq-\mu$. They describe two symmetry-related one-lobe attracting [flow](../../../../../../flow.md) [periodic orbits](../../../../../../periodic-orbit.md). For $\mu>0$, the orbit alternates between $s$ and $-s$, where $s=\mu-As^\delta\simeq\mu$; its multiplier is $(A\delta s^{\delta-1})^2<1$. This represents one attracting [flow](../../../../../../flow.md) [periodic orbit](../../../../../../periodic-orbit.md) traversing both lobes. At $\mu=0$ the two homoclinic loops meet: this is the contracting gluing scenario, with diverging [flow](../../../../../../flow.md) period at the connection.

If $\delta<1$, the local [derivative](../../../../../../derivative.md) is unbounded, and the small [periodic orbits](../../../../../../periodic-orbit.md) are repelling in the expanding return direction. For $\mu>0$, the small positive [fixed point](../../../../../../fixed-point.md) has $s\simeq(\mu/A)^{1/\delta}$, with a multiplier tending to infinity; there is a symmetry-related negative [fixed point](../../../../../../fixed-point.md) as well. More complex motion follows from the two branches, not merely from a large [derivative](../../../../../../derivative.md) at one [fixed point](../../../../../../fixed-point.md). Choose $I=[-c\mu,c\mu]$ with $0<c<1$. The inverse branches are

$$
g_+(y)=((\mu+y)/A)^{1/\delta},\qquad
g_-(y)=-((\mu-y)/A)^{1/\delta}.
$$

For sufficiently small positive $\mu$, both lie inside $I$, their images are disjoint, and their [derivatives](../../../../../../derivative.md) are $O(\mu^{1/\delta-1})\to0$. Nested inverse images for every infinite sign sequence therefore define a Cantor invariant set. Iterating the forward map shifts the sequence. This constructs periodic itineraries of every symbolic period and nonperiodic itineraries; transverse [contraction](../../../../../../contraction-mapping.md) in the full return turns the expanding two-strip mechanism into a horseshoe.

This is the local chaotic Lorenz mechanism. A robust attracting Lorenz set additionally needs a global trapping region and the appropriate return properties. The scalar asymptote and $\delta<1$ alone do not prove that every nearby orbit is attracted to one chaotic set; periodic windows, escaping orbits and other global returns must be distinguished. [Symmetry](../../../../../../symmetry-physics.md) is crucial to obtaining the two homoclinic branches together in a single parameter variation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
