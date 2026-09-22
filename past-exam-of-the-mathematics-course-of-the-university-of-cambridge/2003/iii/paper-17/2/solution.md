<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [symplectic manifold](../../../../../symplectic-manifold.md) is a smooth even-dimensional manifold $X^{2n}$ with a closed, nondegenerate [differential two-form](../../../../../2-form.md) $\omega$. A [Lagrangian submanifold](../../../../../lagrangian-submanifold.md) $L\subset X$ has dimension $n$ and $\omega|_{TL}=0$; equivalently $T_xL=(T_xL)^\omega$ at every point.

On $T^*M$, let $\pi:T^*M\to M$ and define the [canonical one-form on a cotangent bundle](../../../../../canonical-one-form-on-a-cotangent-bundle.md) by $\theta_{(q,p)}(v)=p(d\pi(v))$. In local coordinates $\theta=\sum_i p_i\,dq_i$, so our sign convention gives

$$
\omega_0=-d\theta=\sum_i dq_i\wedge dp_i.
$$

The intrinsic definition of $\theta$ makes this form globally defined. It is closed because $d^2=0$, and its displayed coordinate matrix is invertible. The [zero section](../../../../../zero-section-of-a-vector-bundle.md) pulls $\theta$, and therefore $\omega_0$, back to zero and has half the total dimension. It is a [Lagrangian submanifold](../../../../../lagrangian-submanifold.md).

We prove the [Weinstein neighborhood theorem](../../../../../weinstein-neighborhood-theorem.md), rather than merely invoking it. Along a [Lagrangian submanifold](../../../../../lagrangian-submanifold.md) $L\subset(X,\omega)$, choose a [compatible almost complex structure](../../../../../compatible-almost-complex-structure.md) $J$; its existence is proved by the metric construction in Question 5. Then $JL$ at the tangent-bundle level means $J(TL)$, and

$$
TX|_L=TL\oplus J(TL).
$$

Indeed, $Jv\in TL$ with $v\in TL$ would imply $0=\omega(v,Jv)$, forcing $v=0$. Also $\omega(Ju,Jv)=\omega(u,v)=0$ for $u,v\in TL$, so $J(TL)$ is a [Lagrangian complement](../../../../../lagrangian-complement.md). Identify a normal vector $n\in J(TL)$ with the covector $\eta(v)=\omega(v,n)$. This is a vector-bundle [isomorphism](../../../../../isomorphism.md) with $T^*L$, and under it

$$
\omega((v,\eta),(w,\zeta))=\zeta(v)-\eta(w),
$$

which is exactly the form $\omega_0$ along the [zero section](../../../../../zero-section-of-a-vector-bundle.md). The [tubular neighborhood theorem](../../../../../tubular-neighborhood-theorem.md) therefore supplies a smooth map $F$ from a neighborhood of that section to a neighborhood of $L$, restricting to the identity and with this derivative along $L$.

Write $\omega_1=F^*\omega$ and $\delta=\omega_1-\omega_0$. This [closed differential form](../../../../../closed-differential-form.md) vanishes as an entire [bilinear form](../../../../../bilinear-form.md) along the [zero section](../../../../../zero-section-of-a-vector-bundle.md). The [relative Poincaré lemma](../../../../../relative-poincare-lemma.md) gives $\delta=d\beta$ with $\beta$ zero along the section. Explicitly, if $r_s(q,p)=(q,sp)$ and $R=\sum p_i\partial_{p_i}$, use

$$
\beta=\int_0^1\frac1s r_s^*(\iota_R\delta)\,ds.
$$

The homotopy identity gives $d\beta=\delta-r_0^*\delta=\delta$; the vanishing at the section ensures smoothness of this integral. The forms $\omega_t=\omega_0+t\delta$ are nondegenerate on a sufficiently small neighborhood of the section for all $0\leq t\leq1$. Solve uniquely

$$
\iota_{Y_t}\omega_t=-\beta.
$$

The [vector field](../../../../../vector-field.md) $Y_t$ vanishes on the section. After another neighborhood shrink its [flow](../../../../../flow.md) $\phi_t$ exists up to time one and fixes the section. For noncompact $L$, the sizes of these neighborhoods may vary with the base point; no [compactness](../../../../../compact-space.md) of $L$ is required for the local conclusion. By [Cartan's magic formula](../../../../../cartan-s-magic-formula.md),

$$
\frac d{dt}\phi_t^*\omega_t
=\phi_t^*(\delta+d\iota_{Y_t}\omega_t)=0.
$$

Thus $(F\circ\phi_1)^*\omega=\omega_0$. This establishes the universal neighborhood model, with the [Lagrangian submanifold](../../../../../lagrangian-submanifold.md) identified with the [zero section](../../../../../zero-section-of-a-vector-bundle.md).

For the section $s_\alpha(q)=(q,\alpha_q)$, the canonical [differential one-form](../../../../../one-form.md) satisfies $s_\alpha^*\theta=\alpha$. Hence

$$
\boxed{s_\alpha^*\omega_0=-d\alpha,\qquad\Gamma_\alpha\text{ is Lagrangian}\iff d\alpha=0.}
$$

Its dimension is already half that of $T^*M$, so vanishing of this pullback is sufficient as well as necessary.

Suppose now that a smooth open six-dimensional region were a [fiber bundle](../../../../../fiber-bundle-split.md) with [Lagrangian submanifolds](../../../../../lagrangian-submanifold.md) diffeomorphic to $S^3$ as its fibres. Fix one compact fibre $L$. Smooth local triviality and [compactness](../../../../../compact-space.md) imply that the other sufficiently nearby fibres are $C^1$-close embeddings of $L$. In the [Weinstein neighborhood](../../../../../weinstein-neighborhood-theorem.md), projection to $L$ restricts on each such fibre to a [local diffeomorphism](../../../../../local-diffeomorphism.md) close to the identity. It has degree one, and [compactness](../../../../../compact-space.md) makes it a [covering map](../../../../../covering-space.md), so it is a [diffeomorphism](../../../../../diffeomorphism.md). Each nearby fibre is therefore a graph of a [closed differential one-form](../../../../../closed-differential-one-form.md) $\alpha$ on $S^3$. Since $H^1(S^3;\mathbb R)=0$, this is $df$ for a smooth real function $f$. A maximum of $f$ exists by [compactness](../../../../../compact-space.md), and there $df=0$. The graph meets the original [zero section](../../../../../zero-section-of-a-vector-bundle.md), contradicting disjointness of different fibres. **No such Lagrangian three-sphere fibration exists.** More generally this is the [compact first-cohomology obstruction to a Lagrangian fibration](../../../../../compact-first-cohomology-obstruction-to-a-lagrangian-fibration.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
