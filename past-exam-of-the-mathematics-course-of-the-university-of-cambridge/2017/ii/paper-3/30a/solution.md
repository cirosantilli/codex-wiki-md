<h1 id="30a/solution">Solution</h1>

↑ **Parent:** [30A](../30a.md)

The [centre manifold theorem](../../../../../centre-manifold-theorem.md) gives, near an equilibrium of a sufficiently smooth system, a local invariant [manifold](../../../../../topological-manifold.md) tangent to the [generalized eigenspaces](../../../../../generalized-eigenspace.md) with zero-real-part [eigenvalues](../../../../../eigenvalue.md), expressible as a [graph of a function](../../../../../graph-of-a-function.md) over them. Its reduced dynamics govern local equilibria and their stability in the presence of strictly stable transverse directions. The [manifold](../../../../../topological-manifold.md) need not be unique or analytic; finite Taylor jets can nevertheless be determined from invariance. Treating a parameter as a variable with $\dot\mu=0$ gives the [extended centre manifold for a parameter](../../../../../extended-centre-manifold-for-a-parameter.md).

At $r=1$ the linearized $(x,y)$ block has [eigenvalues](../../../../../eigenvalue.md) $0,-2$, and the $z$ direction has [eigenvalue](../../../../../eigenvalue.md) $-1$. Thus the origin is a [nonhyperbolic equilibrium](../../../../../nonhyperbolic-equilibrium.md), with **stable [dimension](../../../../../dimension-vector-space.md) two and non-extended centre [dimension](../../../../../dimension-vector-space.md) one**. The extended centre [dimension](../../../../../dimension-vector-space.md) is two. The transformed equations are

$$
\begin{aligned}
 \dot u&=\tfrac12\mu(u+v)+\tfrac a2(u+v)^3-\tfrac12(u-v)z,\\
 \dot v&=-2v-\tfrac12\mu(u+v)+\tfrac a2(u+v)^3+\tfrac12(u-v)z,\\
 \dot z&=u^2-v^2-z,\qquad\dot\mu=0.
\end{aligned}
$$

The [graph of a function](../../../../../graph-of-a-function.md) satisfies $V(0,0)=Z(0,0)=0$ and $DV(0,0)=DZ(0,0)=0$, with invariance equations $V_u\dot u=\dot v$ and $Z_u\dot u=\dot z$. Symmetry permits $V$ odd and $Z$ even in $u$. Giving $u$ weight one and $\mu$ weight two, comparison yields

$$
 Z=u^2+O_{\rm w}(4),\qquad
 V=-\frac14\mu u+\frac{a+1}{4}u^3+O_{\rm w}(5),\qquad
 \boxed{\dot u=\frac12\mu u+\frac{a-1}{2}u^3+O_{\rm w}(5).}
$$

Here $O_{\rm w}(j)$ means terms of weighted order at least $j$ under the stated scaling. If $a<1$, the [pitchfork bifurcation](../../../../../pitchfork-bifurcation-normal-form.md) is supercritical: stable branches $u\sim\pm\sqrt{\mu/(1-a)}$ appear for $\mu>0$ as the origin loses stability. If $a>1$, it is a [subcritical pitchfork bifurcation](../../../../../subcritical-pitchfork-bifurcation.md): unstable branches occur for $\mu<0$, while the origin is stable there.

For $a=1$, assign $\mu$ weight four. The leading cubic terms in $\dot u$ cancel. The invariance equations now give $V=u^3/2+O_{\rm w}(5)$ and $Z=u^2+0\,u^4+O_{\rm w}(6)$: $Z_u\dot u$ first contributes at weight six and $v^2$ also first contributes there. Substitution then gives

$$
\boxed{\dot u=\frac12\mu u+u^5+O_{\rm w}(7),\qquad
 u\sim\pm(-\mu/2)^{1/4}\quad(\mu<0).}
$$

The [derivative](../../../../../derivative.md) along the nonzero branches is $-2\mu>0$, so they are unstable. The origin is stable for $\mu<0$, unstable for $\mu>0$, and nonlinearly unstable at $\mu=0$ because the leading term is $+u^5$. This is a degenerate subcritical [pitchfork bifurcation](../../../../../pitchfork-bifurcation-normal-form.md).

<a id="30a/image-bifurcation-diagram-for-the-equilibrium-branches"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3-bifurcation.png)

**[Figure 2](#30a/image-bifurcation-diagram-for-the-equilibrium-branches). Bifurcation diagram for the equilibrium branches**.

## ↑ Ancestors (10)

1. [30A](../30a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
