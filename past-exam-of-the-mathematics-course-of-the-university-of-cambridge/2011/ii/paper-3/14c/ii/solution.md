<h1 id="14c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Near $(1,0)$ put $u=x-1$, $v=y$, $\epsilon=\mu-1$, with $\dot\epsilon=0$. The extended system is

$$
\dot u=-2u-3u^2-u^3-v^2-uv^2,\qquad \dot v=\epsilon v-v^2-2uv-u^2v.
$$

The [extended centre manifold for a parameter](../../../../../../extended-centre-manifold-for-a-parameter.md) has $u=h(v,\epsilon)$, $h(0,0)=0$, $Dh(0,0)=0$. Its [centre-manifold invariance equation](../../../../../../centre-manifold-invariance-equation.md) is $h_v\dot v=\dot u$. The left side starts at degree three. At degree two the right side is $-2h_2-v^2$, so $h_2=-v^2/2$, with no $v\epsilon$ or $\epsilon^2$ term. Substitution gives

$$
\boxed{u=-\tfrac12v^2+O((|v|+|\epsilon|)^3),\qquad \dot v=\epsilon v-v^2+v^3+O((|v|+|\epsilon|)^4).}
$$

The leading [normal form of a dynamical system](../../../../../../normal-form-dynamical-systems.md) $\dot v=\epsilon v-v^2$ has branches $v=0$ and $v\simeq\epsilon$, exchanging stability at $\epsilon=0$: this is a [transcritical bifurcation](../../../../../../transcritical-bifurcation.md). In the physical quadrant the interior branch is present only for $\epsilon>0$.

The equations extended across $x=0$ are equivariant under $x\mapsto-x$, so near $(0,1)$ the reduced equation is odd in $x$. To verify its nondegenerate [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md), set $\eta=\mu-1$ and $z=y-\mu$. Then

$$
\dot x=x[-2\eta-\eta^2-2(1+\eta)z-z^2-x^2],\qquad \dot z=(1+\eta+z)(-z-x^2).
$$

The local centre manifold has $z=-x^2+O(|\eta|x^2+x^4)$, obtained by balancing the quadratic terms of its invariance equation. Consequently $\dot x=-2\eta x+x^3+O(\eta^2|x|+|\eta||x|^3+|x|^5)$: the cubic coefficient is nonzero. This is a subcritical pitchfork, with the two symmetry-related interior branches existing for $\eta>0$ in the extended plane; only the $x>0$ branch belongs to the physical quadrant.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14C](../../14c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
