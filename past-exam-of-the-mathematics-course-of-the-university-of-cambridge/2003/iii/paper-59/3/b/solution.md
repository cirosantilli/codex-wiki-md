<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We count [periodic orbits](../../../../../../periodic-orbit.md) whose trajectories remain near the two specified [homoclinic orbits](../../../../../../homoclinic-orbit.md); the local hypotheses impose no bound on unrelated distant cycles. Choose the return domain small enough that $A\delta|x|^{\delta-1}$ and $B\delta|x|^{\delta-1}$ are less than one. Each admissible return branch is then a [contraction mapping](../../../../../../contraction-mapping.md).

A right-lobe [periodic orbit](../../../../../../periodic-orbit.md) is a [fixed point](../../../../../../fixed-point.md) $(p,+1)$ with $p>0$ and $p=-\mu+Ap^\delta$. For small amplitudes it exists exactly when $\mu<0$, and $p=-\mu+o(|\mu|)$. Similarly, a left-lobe [periodic orbit](../../../../../../periodic-orbit.md) has $(x,y)=(-q,-1)$, $q>0$, $q=-\nu+Bq^\delta$, and exists for $\nu<0$. Their [Floquet multipliers](../../../../../../floquet-multiplier.md) tend to zero, so both are attracting.

A [period-two orbit](../../../../../../period-two-orbit.md) of the section map corresponds to one flow [periodic orbit](../../../../../../periodic-orbit.md) traversing both lobes. Write its states as $(p,-1)$ and $(-q,+1)$. Its positive amplitudes satisfy

$$
\boxed{q=\mu+Ap^\delta,\qquad p=\nu+Bq^\delta.}
$$

The two-step derivative is $AB\delta^2p^{\delta-1}q^{\delta-1}$, again tending to zero. The [asymmetric planar gluing return map](../../../../../../asymmetric-planar-gluing-return-map.md) therefore gives at most one such attracting two-lobe cycle in the small domain. Its boundaries are obtained by setting one amplitude to zero:

$$
\boxed{C_R:\ \mu=-A\nu^\delta\ (\nu>0),\qquad
C_L:\ \nu=-B\mu^\delta\ (\mu>0).}
$$

For the original flow these are leading equations, with corrections $o(\nu^\delta)$ or $o(\mu^\delta)$. On $C_R$, the negative unstable branch makes both excursions before returning to the positive stable branch; on $C_L$ the positive unstable branch returns to the negative stable branch. Each is a compound [homoclinic orbit](../../../../../../homoclinic-orbit.md), with one extra passage near the [saddle equilibrium](../../../../../../saddle-equilibrium.md). They are distinct from the primary loop curves $\mu=0$ and $\nu=0$.

The six open regions and their local cycles are:

| Region | Attracting flow cycles |
| --- | --- |
| $\mu<0,\ \nu<0$ | Right and left single-lobe cycles |
| $\nu>0,\ \mu<-A\nu^\delta$ | Right single-lobe cycle only |
| $\nu>0,\ -A\nu^\delta<\mu<0$ | Right single-lobe cycle and two-lobe cycle |
| $\mu>0,\ \nu<-B\mu^\delta$ | Left single-lobe cycle only |
| $\mu>0,\ -B\mu^\delta<\nu<0$ | Left single-lobe cycle and two-lobe cycle |
| $\mu>0,\ \nu>0$ | Two-lobe cycle only |

There is no additional small alternating cycle when both parameters are negative. Indeed the two positive-amplitude equations would imply $q<Ap^\delta$ and $p<Bq^\delta$, giving $p<BA^\delta p^{\delta^2}$, impossible for sufficiently small positive $p$. On each mixed-sign quadrant the contraction equations give the two-lobe cycle precisely on the side of the compound curve toward the positive quadrant.

On $\mu=0$, there is the primary right [homoclinic orbit](../../../../../../homoclinic-orbit.md), together with a left cycle if $\nu<0$ or a two-lobe cycle if $\nu>0$. On $\nu=0$ the analogous statement holds with left and right interchanged. On $C_R$ there is a compound [homoclinic orbit](../../../../../../homoclinic-orbit.md) and the right single-lobe cycle; on $C_L$ there is a compound [homoclinic orbit](../../../../../../homoclinic-orbit.md) and the left single-lobe cycle. At $(0,0)$ the two primary loops meet at the same [saddle equilibrium](../../../../../../saddle-equilibrium.md). The approach to each [homoclinic orbit](../../../../../../homoclinic-orbit.md) has a diverging period; it is not a saddle-node collision of two finite-period cycles.

<a id="3/b/image-parameter-regions-and-schematic-phase-portraits-for-asymmetric-planar-gluing"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-59-gluing-regions.png)

**[Figure 3](#3/b/image-parameter-regions-and-schematic-phase-portraits-for-asymmetric-planar-gluing). Parameter regions and schematic phase portraits for asymmetric planar gluing**.

<a id="3/b/image-primary-compound-and-double-homoclinic-connections-on-every-global-bifurcation-curve"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-59-gluing-connections.png)

**[Figure 4](#3/b/image-primary-compound-and-double-homoclinic-connections-on-every-global-bifurcation-curve). Primary, compound, and double homoclinic connections on every global bifurcation curve**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
