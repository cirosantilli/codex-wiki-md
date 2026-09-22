<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A smooth [vector field along a map](../../../../../vector-field-along-a-map.md) $\gamma:[a,b]\to M$ is a smooth section of the [pullback tangent bundle](../../../../../pullback-tangent-bundle.md) $\gamma^*TM$: it assigns $V(t)\in T_{\gamma(t)}M$, with smooth coefficients in each local frame. It need not be the restriction of one ambient [vector field](../../../../../vector-field.md), since a curve may return to the same point with different values of $V$.

An [affine connection](../../../../../affine-connection.md), also called a [Koszul connection](../../../../../affine-connection.md), induces a [pullback connection](../../../../../pullback-connection.md) on this bundle. In coordinates, write $V=V^i(t)\partial_i$ and $\nabla_{\partial_j}\partial_k=\Gamma^i{}_{jk}\partial_i$. Its [covariant derivative along a curve](../../../../../covariant-derivative-along-a-curve.md) is

$$
D_tV=\left(\dot V^i+\Gamma^i{}_{jk}(\gamma(t))\dot\gamma^jV^k\right)\partial_i.
$$

The connection transformation law, or the [Leibniz rule](../../../../../leibniz-rule.md) applied to a change of frame, makes this expression independent of the frame. In particular it is defined even when $\dot\gamma=0$; it differentiates the section's coefficients as well as the frame.

The field is parallel precisely when $D_tV=0$. In a frame along a coordinate segment this is the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md)

$$
\dot V^i=-A^i{}_k(t)V^k,\qquad
A^i{}_k(t)=\Gamma^i{}_{jk}(\gamma(t))\dot\gamma^j(t).
$$

The [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) gives a unique solution with prescribed initial value. Smooth coefficients on compact subintervals are bounded, and the usual norm estimate for a [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) prevents finite-time blowup there. A finite sequence of coordinate segments covers the image of the compact interval $[a,b]$; solve successively and use uniqueness on overlaps. This gives a unique parallel field on the whole interval for every $V_a\in T_{\gamma(a)}M$.

Define [parallel transport](../../../../../parallel-transport.md) by $\tau_t(V_a)=V(t)$. Linearity of the equation and uniqueness give $\tau_t(cV_a+dW_a)=c\tau_t(V_a)+d\tau_t(W_a)$. Solving along the reversed curve supplies its inverse. Therefore **each $\tau_t:T_{\gamma(a)}M\to T_{\gamma(t)}M$ is a linear isomorphism**.

For two [affine connections](../../../../../affine-connection.md), put $\Delta(X,Y)=\nabla_XY-\widetilde\nabla_XY$. Their rules give

$$
\Delta(fX,Y)=f\Delta(X,Y),\qquad
\Delta(X,fY)=f\Delta(X,Y),
$$

since the two $X(f)Y$ terms cancel. The [tensoriality](../../../../../tensoriality.md) of this operation proves that the [difference of affine connections is a tensor](../../../../../difference-of-affine-connections-is-a-tensor.md), of type $(1,2)$, with smooth coordinate coefficients $\Gamma^i{}_{jk}-\widetilde\Gamma^i{}_{jk}$.

A parametrized [geodesic](../../../../../geodesic.md) satisfies $D_t\dot\gamma=0$, or the [geodesic equation](../../../../../geodesic-equation.md)

$$
\ddot\gamma^i+\Gamma^i{}_{jk}(\gamma)\dot\gamma^j\dot\gamma^k=0.
$$

With $v^i=\dot\gamma^i$, this becomes the first-order system $\dot\gamma^i=v^i$, $\dot v^i=-\Gamma^i{}_{jk}(\gamma)v^jv^k$. Its right side is smooth, so the [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) gives a unique local solution for each initial point and tangent vector. This establishes uniqueness with the parametrization fixed.

The two accelerations differ by

$$
D_t\dot\gamma-\widetilde D_t\dot\gamma=\Delta(\dot\gamma,\dot\gamma).
$$

If $\Delta(v,v)=0$ for every tangent vector, either acceleration vanishes exactly when the other does. Conversely, start the $\nabla$-[geodesic](../../../../../geodesic.md) with arbitrary initial vector $v$ at an arbitrary point. If it is also a $\widetilde\nabla$-[geodesic](../../../../../geodesic.md) with the same parameter, evaluating this identity initially gives $\Delta(v,v)=0$. Hence

$$
\boxed{\text{same parametrized geodesics}\quad\Longleftrightarrow\quad
\Delta(v,v)=0\text{ for every }v}.
$$

Polarization makes the latter condition equivalent to $\Delta(u,v)+\Delta(v,u)=0$: [parametrized geodesics determine the symmetric part of an affine connection](../../../../../parametrized-geodesics-determine-the-symmetric-part-of-an-affine-connection.md). In particular [torsion-free connections are determined by their parametrized geodesics](../../../../../torsion-free-connections-are-determined-by-their-parametrized-geodesics.md), since their difference is also symmetric and must then vanish.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
