<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Minkowski metric](../../../../../minkowski-metric.md) with signature $(+,-)$, and write $V(\phi)=\tfrac12(1-\phi^2)^2$. The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\partial_\mu\partial^\mu\phi+V'(\phi)=0,
\qquad\boxed{\phi_{tt}-\phi_{xx}+2\phi(\phi^2-1)=0.}
$$

For the static [phi-four kink](../../../../../phi-four-kink.md), $\phi_x=1-\phi^2=\operatorname{sech}^2(x-a)$ and $\phi_{xx}=-2\phi(1-\phi^2)=2\phi(\phi^2-1)$, so the field equation is satisfied. The centre $a$ is arbitrary by [translation invariance](../../../../../translation-invariance.md), and the [hyperbolic tangent](../../../../../hyperbolic-tangent.md) profile increases monotonically from $-1$ to $+1$, crossing zero at $x=a$. **The static [kink](../../../../../scalar-field-kink.md) and its endpoint [topological charge](../../../../../topological-charge.md) are**

$$
\boxed{\phi_K(x)=\tanh(x-a),\qquad Q=\frac{\phi(+\infty)-\phi(-\infty)}2=1.}
$$

<a id="1/image-the-phi-four-kink-rises-between-the-two-vacuum-values-and-crosses-zero-at-its-centre"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-308-kink.png)

**[Figure 1](#1/image-the-phi-four-kink-rises-between-the-two-vacuum-values-and-crosses-zero-at-its-centre). The phi-four kink rises between the two vacuum values and crosses zero at its centre**.

Both endpoint values are isolated [classical vacua](../../../../../classical-vacuum.md), since $V(\phi)=0$ only at $\phi=\pm1$. A continuous finite-energy deformation preserving the vacuum boundary conditions cannot change either endpoint to the other isolated [classical vacuum](../../../../../classical-vacuum.md). The [topological charge](../../../../../topological-charge.md) is therefore unchanged: this [kink](../../../../../scalar-field-kink.md) cannot deform into a homogeneous [classical vacuum](../../../../../classical-vacuum.md), whose charge is zero. There is also a direct [Bogomolny bound](../../../../../bogomolny-bound.md) in this sector. The [square completion for a one-dimensional kink](../../../../../square-completion-for-a-one-dimensional-kink.md) gives

$$
\begin{aligned}
E&=\int_{\mathbb R}\left[\frac12\phi_t^2+\frac12\phi_x^2+V(\phi)\right]dx\\
&=\int_{\mathbb R}\left[\frac12\phi_t^2+\frac12\big(\phi_x-(1-\phi^2)\big)^2\right]dx
+\left[\phi-\frac{\phi^3}{3}\right]_{-\infty}^{+\infty}
\geq\frac43.
\end{aligned}
$$

The [phi-four kink](../../../../../phi-four-kink.md) saturates the bound, so its mass is $4/3$ in these units and it minimizes the energy within its [topological sector](../../../../../topological-sector.md). Its arbitrary position is a [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md), not an instability. A [kink](../../../../../scalar-field-kink.md) and an [antikink](../../../../../antikink.md) together have total charge zero and can annihilate without contradicting the protection of an isolated [kink](../../../../../scalar-field-kink.md).

For the momentum, the [canonical stress-energy tensor](../../../../../canonical-stress-energy-tensor.md) of this [scalar field](../../../../../scalar-field.md) is

$$
T^{\mu\nu}=\partial^\mu\phi\,\partial^\nu\phi-\eta^{\mu\nu}\mathcal L.
$$

Consequently the physical spatial [momentum density](../../../../../momentum-density.md) and the spatial momentum flux are

$$
\boxed{\mathcal P=T^{01}=-\phi_t\phi_x,\qquad
T^{11}=\frac12\phi_t^2+\frac12\phi_x^2-V(\phi).}
$$

The sign of $\mathcal P$ makes a right-moving translated [kink](../../../../../scalar-field-kink.md) carry positive momentum. Direct use of the field equation, rather than an assumed static field, yields the [scalar-field momentum flux](../../../../../scalar-field-momentum-flux.md) identity

$$
\partial_t\mathcal P
=-\phi_{tt}\phi_x-\phi_t\phi_{xt}
=\partial_x\!\left[V(\phi)-\frac12\phi_x^2-\frac12\phi_t^2\right]
=-\partial_xT^{11}.
$$

The [finite-energy field configuration](../../../../../finite-energy-field-configuration.md) has $\mathcal P\in L^1$ by $|\phi_t\phi_x|\leq(\phi_t^2+\phi_x^2)/2$. Integrating the [stress-energy conservation](../../../../../stress-energy-conservation.md) law over the left half-line gives **the boundary [force](../../../../../force.md)**

$$
\boxed{\frac{d}{dt}\int_{-\infty}^b\mathcal P\,dx
=-T^{11}(b,t)
=\left[V(\phi)-\frac12\phi_x^2-\frac12\phi_t^2\right]_{x=b}.}
$$

Under the usual vacuum falloff, the stress at the left endpoint is zero. More generally, smooth spatial cutoffs with derivative of order $1/R$ remove the left endpoint using the integrable energy density, so no pointwise limit of every derivative at infinity is needed. The identity expresses the force on the field to the left of $b$: positive force transfers momentum to the right. For well separated solitons, a cut between them measures the interaction force on the left soliton.

Take that cut at $b=0$. The specified symmetric pair has, at the initial time,

$$
\phi(0)=2\tanh c-1,\qquad\phi_x(0)=0.
$$

The printed field profile does not itself specify the initial velocity. If $\psi(x)=\phi_t(x,0)$, the exact initial half-line force is

$$
F_{\rm left}(0)=8\tanh^2c\,(1-\tanh c)^2-\frac12\psi(0)^2.
$$

For the intended initially resting pair, or more generally $\psi(0)=0$, put $q=e^{-2c}$ and use $\tanh c=(1-q)/(1+q)$. The [at-rest force for a symmetric phi-four pair](../../../../../at-rest-force-for-a-symmetric-phi-four-pair.md) is

$$
F_K=\frac{32q^2(1-q)^2}{(1+q)^4}
=32e^{-4c}+O(e^{-6c}).
$$

**The leading [force](../../../../../force.md) is attractive, towards the [antikink](../../../../../antikink.md)**:

$$
\boxed{F_K\sim+32e^{-4c}=32e^{-2d},\qquad d=2c.}
$$

The [antikink](../../../../../antikink.md) feels the opposite force by the symmetry of the resting pair. This is an initial, large-separation interaction calculation, not a claim that the superposed profile is an exact static two-soliton solution. Without the initial-velocity condition, the additional momentum flux above prevents a unique force from being inferred from the printed profile alone.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
