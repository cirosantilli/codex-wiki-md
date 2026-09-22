<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

One definition of $T_xM$ is the space of derivations at $x$: linear maps $v:C^\infty(M)\to\mathbb R$ satisfying $v(fh)=f(x)v(h)+h(x)v(f)$. In local coordinates $u^1,\ldots,u^n$, each has the unique form $v=\sum_iv^i\partial/\partial u^i|_x$, identifying $T_xM$ with $\mathbb R^n$. Equivalently it is the space of velocities of curves through $x$, identifying curves with the same coordinate derivative.

For a chart $\phi:U\to\mathbb R^n$, give $TM|_U$ coordinates $(x,v)\mapsto(\phi(x),D\phi_xv)$. If $F=\psi\circ\phi^{-1}$ is a base transition, the induced transition is

$$
(u,v)\longmapsto(F(u),DF_u v).
$$

This is a smooth bijection with smooth inverse coming from the reverse chart. The resulting bundle atlas makes $TM$ a [smooth manifold](../../../../smooth-manifold-split.md) of dimension $2n$. These local product charts also give the usual [Hausdorff](../../../../hausdorff-space.md) and second-countable [topology](../../../../topology-split.md), inherited from a countable base atlas and its fibre coordinates.

For $n\ge1$, identify nonzero vectors in each fibre up to nonzero real scalar multiplication. Locally this gives $P(TM)|_U\cong U\times\mathbb{RP}^{n-1}$. In a projective chart where $v^j\ne0$, use the ratios $v^i/v^j$ for $i\ne j$. Under a base change, the fibre line maps by $[v]\mapsto[DF_uv]$; its projective coordinates are ratios of smooth linear expressions with nonzero denominator on the overlap. This defines a [smooth manifold](../../../../smooth-manifold-split.md) of dimension $n+(n-1)=2n-1$.

For the sphere, a point is a pair $(x,L)$ with $|x|=1$ and an unoriented line $L\subset x^\perp$. Choose a unit $v\in L$. The triple $(x,v,x\times v)$ is a positively oriented orthonormal frame. Given a second pair, the unique [orientation](../../../../orientation-of-a-simplex.md)-preserving linear map between chosen frames lies in $SO_3$ and carries the first pair to the second. Thus the action is transitive.

A rotation stabilizing $(x,L)$ fixes $x$, so rotates its tangent plane. To preserve the unoriented line it must act by $v\mapsto v$ or $v\mapsto-v$, giving exactly the identity and a half-turn about $x$. Hence **the [stabilizer](../../../../stabilizer-subgroup.md) has order two**, and $P(TS^2)\cong SO_3/C_2$.

This is an example of the [projectivized tangent bundle](../../../../projectivized-tangent-bundle.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the lie Groups and Differentiable Manifolds course of the University of Oxford](../../../split.md)
5. [Lie Groups and Differentiable Manifolds course of the University of Oxford](../../../../lie-groups-and-differentiable-manifolds-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
