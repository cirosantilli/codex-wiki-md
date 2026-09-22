<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We prove the [Weinstein neighborhood theorem](../../../../../weinstein-neighborhood-theorem.md) with the canonical sign convention $\omega_0=-d\alpha$. The essential first step is to match the two [symplectic forms](../../../../../symplectic-form.md) as bilinear forms on the entire tangent space along $X$, not only after pulling them back to $TX$.

Here is the needed [symplectic splitting along a Lagrangian submanifold](../../../../../symplectic-splitting-along-a-lagrangian-submanifold.md). Write $E=TM|_X$ and $L=TX$. Choose a smooth [vector bundle](../../../../../vector-bundle.md) complement $N$ of $L$, for example using a [Riemannian metric](../../../../../riemannian-metric.md). Since $L$ is a [Lagrangian subspace](../../../../../lagrangian-subspace.md) in every fiber, the pairing map

$$
N\longrightarrow L^*,\qquad v\longmapsto\bigl(u\longmapsto\omega(u,v)\bigr)
$$

is an isomorphism: its kernel is $N\cap L^\omega=N\cap L=0$, and both bundles have rank $n$. Let $s:L^*\to N$ be its inverse and put $b(\eta,\zeta)=\omega(s\eta,s\zeta)$. Define $a:L^*\to L$ by

$$
\zeta(a\eta)=-\tfrac12 b(\eta,\zeta),
$$

and set $\widetilde s=s+a$. Nondegeneracy of the dual pairing gives a unique smooth $a$. Since $b$ is alternating,

$$
\omega(\widetilde s\eta,\widetilde s\zeta)
=b(\eta,\zeta)-\eta(a\zeta)+\zeta(a\eta)=0.
$$

Thus $K=\widetilde s(L^*)$ is a smooth [Lagrangian complement](../../../../../lagrangian-complement.md) to $L$. The map

$$
A:TX\oplus T^*X\longrightarrow TM|_X,\qquad
A(u,\eta)=u+\widetilde s\eta
$$

is a [vector bundle isomorphism](../../../../../vector-bundle-isomorphism.md), is the identity on $TX$, and satisfies

$$
\omega(A(u,\eta),A(v,\zeta))=\zeta(u)-\eta(v)
=\omega_0((u,\eta),(v,\zeta)).
$$

The last equality uses the canonical splitting of the tangent bundle of $T^*X$ along its [zero section](../../../../../zero-section-of-a-vector-bundle.md).

Choose a [Riemannian metric](../../../../../riemannian-metric.md) near $X$ for which $K$ is orthogonal to $TX$. The [tubular neighborhood](../../../../../tubular-neighborhood.md) construction using its [Riemannian exponential map](../../../../../exponential-map-riemannian-geometry.md) gives a [diffeomorphism](../../../../../diffeomorphism.md)

$$
\psi:W\subset T^*X\longrightarrow W'\subset M,\qquad
\psi(q,p)=\exp_q(\widetilde s_qp),
$$

after shrinking around the [zero section](../../../../../zero-section-of-a-vector-bundle.md). It restricts to the given inclusion of $X$ and has differential $A$ along it. Consequently $\beta=\psi^*\omega$ and $\omega_0$ agree pointwise as ambient bilinear forms at every point of the [zero section](../../../../../zero-section-of-a-vector-bundle.md).

We use the following precise [relative Moser theorem](../../../../../relative-moser-theorem.md). If two closed [symplectic forms](../../../../../symplectic-form.md) $\gamma_0,\gamma_1$ near a compact embedded submanifold $S$ agree as ambient bilinear forms along $S$, then, on smaller neighborhoods, there is a [diffeomorphism](../../../../../diffeomorphism.md) $\kappa$ fixing $S$ pointwise with $\kappa^*\gamma_1=\gamma_0$. One sufficient version allows a symplectic path $\gamma_t$ with $\partial_t\gamma_t=d\eta_t$ and $\eta_t=0$ as ambient covectors along $S$: solve $\iota_{Z_t}\gamma_t=-\eta_t$ and use its flow. The [vector field](../../../../../vector-field.md) vanishes on $S$, so the flow fixes $S$, and compactness permits a common smaller neighborhood for the full time interval.

For completeness, all hypotheses can be checked directly here. Put $\delta=\beta-\omega_0$ and $\gamma_t=\omega_0+t\delta$. At the [zero section](../../../../../zero-section-of-a-vector-bundle.md), every $\gamma_t$ equals $\omega_0$. The [nondegenerate](../../../../../nondegenerate-bilinear-form.md) property is open, and compactness of $X\times[0,1]$ allows a single smaller neighborhood on which all $\gamma_t$ are [symplectic forms](../../../../../symplectic-form.md). Choose it fiberwise star-shaped. Write $H_s(q,p)=(q,sp)$ and let $E$ be the vertical radial [vector field](../../../../../vector-field.md). The [radial homotopy primitive near a zero section](../../../../../radial-homotopy-primitive-near-a-zero-section.md)

$$
\eta=\int_0^1 s^{-1}H_s^*(\iota_E\delta)\,ds
$$

is smooth, is zero as an ambient covector along the [zero section](../../../../../zero-section-of-a-vector-bundle.md), and satisfies

$$
d\eta=\delta-H_0^*\delta=\delta.
$$

The [radial homotopy operator](../../../../../radial-homotopy-operator.md) gives this identity, using $d\delta=0$ and $H_0^*\delta=\pi^*i_0^*\delta=0$. Smoothness at $s=0$ follows because contraction with $E$ supplies a factor of $s$ after evaluation at $(q,sp)$; the vanishing of $\delta$ along $X$ supplies additional vanishing. Therefore solve $\iota_{Z_t}\gamma_t=-\eta$. By [Cartan's magic formula](../../../../../cartan-s-magic-formula.md), its [flow maps](../../../../../flow-map.md) $\kappa_t$ satisfy

$$
\frac d{dt}(\kappa_t^*\gamma_t)
=\kappa_t^*\bigl(\delta+d(\iota_{Z_t}\gamma_t)\bigr)=0.
$$

After shrinking the starting neighborhood, these flows exist for $0\leq t\leq1$ and fix $X$. This is a relative local construction, not an assertion of completeness throughout the noncompact [cotangent bundle](../../../../../cotangent-bundle.md).

Finally set $\varphi=\psi\circ\kappa_1$, let $U_0$ be its sufficiently small domain, and let $U=\varphi(U_0)$. Then

$$
\boxed{\varphi^*\omega=\kappa_1^*\beta=\omega_0,
\qquad \varphi\circ i_0=i.}
$$

Thus the map is a [symplectomorphism](../../../../../symplectomorphism.md) of neighborhoods and agrees with the specified inclusion at every point of $X$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
