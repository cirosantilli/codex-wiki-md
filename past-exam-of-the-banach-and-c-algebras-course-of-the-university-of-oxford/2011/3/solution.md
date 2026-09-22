<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A **[state on a C-star algebra](../../../state-on-a-c-star-algebra.md)** is a positive [linear functional](../../../linear-functional.md) of [norm](../../../norm.md) one. In the unital case this is equivalent to positivity and $x(1)=1$. A unital star-homomorphism $\pi:A\to\mathcal B(K)$ is a **[cyclic representation of a C-star algebra](../../../cyclic-representation-of-a-c-star-algebra.md)** if it has a [vector](../../../vector.md) $\xi$ with $\overline{\pi(A)\xi}=K$. For the representation associated with a state, the cyclic [vector](../../../vector.md) is taken to have [norm](../../../norm.md) one.

Use [inner products](../../../inner-product-split.md) linear in the first argument, as in the displayed formula for the projection in the source. In the **[Gelfand–Naimark–Segal construction](../../../gelfand-naimark-segal-construction.md)**, set

$$
N_x=\{a\in A:x(a^*a)=0\},\qquad
\langle[a],[b]\rangle=x(b^*a).
$$

The [Cauchy–Schwarz inequality for positive C-star functionals](../../../cauchy-schwarz-inequality-for-positive-c-star-functionals.md) makes this [inner product](../../../inner-product-split.md) well-defined on $A/N_x$. Indeed a null [vector](../../../vector.md) pairs to zero with every [vector](../../../vector.md). The set $N_x$ is a [left ideal](../../../left-ideal.md): $c^*c\leq\|c\|^21$ implies

$$
x((ca)^*(ca))\leq\|c\|^2x(a^*a),
$$

so $a\in N_x$ implies $ca\in N_x$. The same estimate shows that left multiplication induces a [bounded operator](../../../continuous-linear-operator.md)

$$
\pi_x(c)[a]=[ca],\qquad\|\pi_x(c)\|\leq\|c\|.
$$

Complete the quotient pre-Hilbert space to $H_x$, and extend these operators by [continuity](../../../continuous-function.md). The formula for the [inner product](../../../inner-product-split.md) gives $\pi_x(c)^*=\pi_x(c^*)$, while multiplication and the unit are preserved. Put $\xi_x=[1]$. Then $\|\xi_x\|=1$, the [vectors](../../../vector.md) $\pi_x(a)\xi_x=[a]$ are dense in $H_x$, and

$$
\boxed{x(a)=\langle\pi_x(a)\xi_x,\xi_x\rangle.}
$$

This gives the requested cyclic representation for an arbitrary state.

For the specified unit [vector](../../../vector.md) $\eta$, the functional $x_\eta$ is complex-linear and obeys $|x_\eta(a)|\leq\|a\eta\|\|\eta\|\leq\|a\|$. Moreover

$$
x_\eta(1)=1,\qquad x_\eta(a^*a)=\|a\eta\|^2\geq0.
$$

Thus it is positive and has [norm](../../../norm.md) exactly one, proving that **$x_\eta$ is a [vector state on a C-star algebra](../../../vector-state-on-a-c-star-algebra.md)**.

The rank-one projection satisfies

$$
(ap_\eta)(\zeta)=\langle\zeta,\eta\rangle a\eta.
$$

If $a\eta=0$, this is zero for every $\zeta$, so $ap_\eta=0$. Conversely, evaluation at $\zeta=\eta$ gives $(ap_\eta)\eta=a\eta$. Hence

$$
\boxed{a\eta=0\quad\Longleftrightarrow\quad ap_\eta=0.}
$$

In particular $N_{x_\eta}=\{a:a\eta=0\}=\{a:ap_\eta=0\}$.

The concrete GNS space is the [completion](../../../hilbert-space-completion.md) of $A/N_{x_\eta}$ with

$$
\langle[a],[b]\rangle=x_\eta(b^*a)=\langle a\eta,b\eta\rangle.
$$

Define $U_0[a]=a\eta$. The description of the null ideal proves it is well-defined, and the displayed equality proves it is a [linear isometry](../../../linear-isometry-of-hilbert-spaces.md) with range $A\eta$. It therefore extends to an [isometry](../../../isometry.md) $U:H_{x_\eta}\to\overline{A\eta}$. The extended range is closed, since its domain is complete, and contains the dense set $A\eta$. Thus **$U$ is onto the required [closure](../../../closure-topology.md)**.

In fact here $A=\mathcal B(H)$, so $A\eta=H$: given any $\zeta\in H$, the bounded rank-one operator $b(v)=\langle v,\eta\rangle\zeta$ sends $\eta$ to $\zeta$. Thus $U$ is a unitary map onto all of $H$, and $U\xi_{x_\eta}=\eta$.

Finally, on the dense quotient [vectors](../../../vector.md),

$$
U\pi_{x_\eta}(a)[b]=U[ab]=ab\eta=aU[b].
$$

Both sides are [bounded operators](../../../continuous-linear-operator.md), so this identity extends to all of $H_{x_\eta}$. Multiplication by the inverse unitary map gives

$$
\boxed{\pi_{x_\eta}(a)=U^{-1}aU\qquad(a\in A).}
$$

This is the [GNS representation of a vector state](../../../gns-representation-of-a-vector-state.md), with the [vector](../../../vector.md) state, null ideal, cyclic [vector](../../../vector.md) and intertwining [isometry](../../../isometry.md) all made explicit.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2011](../../2011-split.md)
3. [Past exam of the Banach and C\*-algebras course of the University of Oxford](../../split.md)
4. [Banach and C\*-algebras course of the University of Oxford](../../../banach-and-c-algebras-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
