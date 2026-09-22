<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [local flow](../../../../../../local-flow.md) of $X$ is the smooth map $\Phi:D\to M$, where $D\subset\mathbb R\times M$ is the maximal open domain of initial-point/time pairs, whose curve $t\mapsto\Phi(t,q)=\phi_t(q)$ is the maximal [integral curve of a vector field](../../../../../../integral-curve-of-a-vector-field.md) through $q$, with $\phi_0(q)=q$. Smooth dependence in the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) theorem gives joint smoothness and openness of $D$. Each time slice is a [diffeomorphism](../../../../../../diffeomorphism.md) between its domain and image, with inverse $\phi_{-t}$.

Here is the group law, including its domain qualification. Fix $s,q$ where the relevant trajectories exist. Both curves

$$
t\longmapsto\phi_{t+s}(q),
\qquad
t\longmapsto\phi_t(\phi_s(q))
$$

solve the same autonomous [ordinary differential equation](../../../../../../ordinary-differential-equation.md) and have value $\phi_s(q)$ at $t=0$. The uniqueness from the first part therefore gives

$$
\boxed{\phi_{t+s}(q)=\phi_t(\phi_s(q))}
$$

on their common interval. These are local identities; neither the [vector field](../../../../../../vector-field.md) nor its [local flow](../../../../../../local-flow.md) has been assumed complete.

For the commuting [local flows](../../../../../../local-flow.md) $\phi_t$ and $\psi_s$, differentiate $\phi_t(\psi_s(q))=\psi_s(\phi_t(q))$ with respect to $s$ at zero. The [chain rule](../../../../../../chain-rule.md) gives

$$
\boxed{(D_q\phi_t)Y_q=Y_{\phi_t(q)}.}
$$

Thus the [pushforward of a vector field](../../../../../../pushforward-of-a-vector-field.md) $Y$ by the $X$ flow equals $Y$. Interchanging the two fields gives the analogous identity for $X$ under $\psi_s$.

Now let $\mathcal D_q=\operatorname{span}(X_q,Y_q)$. Pointwise [linear independence](../../../../../../linear-independence.md) makes this a rank-two [smooth distribution](../../../../../../distribution-differential-geometry.md). The identity just proved implies $[X,Y]=0$: in coordinates, differentiating $D_q\phi_tY_q=Y_{\phi_t(q)}$ at $t=0$ gives $DX(q)Y_q=DY(q)X_q$, precisely the vanishing [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md). The bracket of two local sections is also in $\mathcal D$, since

$$
[fX,gY]=fg[X,Y]+fX(g)Y-gY(f)X
$$

and the analogous terms for $[fX,gX]$ and $[fY,gY]$ remain in the same span. Therefore $\mathcal D$ is an [involutive distribution](../../../../../../involutive-distribution.md).

The [Frobenius theorem](../../../../../../frobenius-theorem.md) says that a smooth constant-rank involutive distribution has local coordinates $(u^1,\ldots,u^n)$ in which it is spanned by $\partial_{u^1},\partial_{u^2}$, and has unique maximal connected [integral manifolds](../../../../../../integral-manifold.md) through its points. These are the [leaves of a regular foliation](../../../../../../leaf-of-a-regular-foliation.md). Let $S$ be the maximal leaf through $p$. The [global confinement to an immersed leaf](../../../../../../global-confinement-to-an-immersed-leaf.md) gives the answer: **$S$ is a two-dimensional immersed integral manifold and every smooth $\mathcal D$-tangent curve starting at $p$ stays in $S$.**

For the curve assertion, in each Frobenius chart the transverse coordinate functions $u^3,\ldots,u^n$ have zero derivative along such a curve. Hence its segment in that chart stays in one plaque. On any compact subinterval of the curve's parameter interval, a finite chain of overlapping such segments connects the initial plaque to the last; all belong to the same maximal leaf. Exhausting the parameter interval proves the assertion for every time.

The two commuting [local flows](../../../../../../local-flow.md) also give the leaf parametrization directly near $p$:

$$
F(s,t)=\phi_s(\psi_t(p)).
$$

Its partial derivatives are $\partial_sF=X_F$ and $\partial_tF=Y_F$, by the pushforward identity. Its differential has rank two. The [constant rank theorem](../../../../../../constant-rank-theorem.md) makes a sufficiently small image an embedded local plaque with tangent plane $\mathcal D$. This is a concrete local construction of the [integral manifold](../../../../../../integral-manifold.md).

There is a global distinction in the word “submanifold”. If it is required to mean an [embedded submanifold](../../../../../../embedded-submanifold.md), the assertion for all times is not valid in general. On the [three-dimensional torus](../../../../../../three-dimensional-torus.md) $\mathbb R^3/\mathbb Z^3$, take

$$
X=\partial_x+\alpha\partial_z,\qquad Y=\partial_y,\qquad \alpha\notin\mathbb Q.
$$

The fields are independent and commute, and their [dense immersed cylinder in a three-dimensional torus](../../../../../../dense-immersed-cylinder-in-a-three-dimensional-torus.md) through zero is

$$
S=\{(s,t,\alpha s)\bmod\mathbb Z^3:s,t\in\mathbb R\}.
$$

It is an injectively immersed cylinder $\mathbb R\times(\mathbb R/\mathbb Z)$ and is dense in the torus. Indeed, fixing $x\bmod1$ and varying $s$ by integers makes $\alpha s\bmod1$ dense by an [irrational rotation of the circle](../../../../../../irrational-rotation.md); $t$ is unrestricted. Every point of this leaf is reached by a tangent curve $r\mapsto(rs,rt,\alpha rs)\bmod\mathbb Z^3$. An embedded surface containing it would, in a submanifold chart near one of its points, be a closed coordinate plane containing a dense subset of the ambient open chart, an impossibility. Thus the global conclusion uses an immersed leaf; the embedded conclusion is local, for curve segments remaining in a suitable chart.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
