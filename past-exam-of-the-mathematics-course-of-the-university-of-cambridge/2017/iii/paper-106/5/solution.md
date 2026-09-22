<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) identifies the dual of the complex [space of continuous functions on a compact space](../../../../../space-of-continuous-functions-on-a-compact-space.md) $C(K)$ with finite regular complex [Borel measures](../../../../../borel-measure.md) on $K$: each [bounded linear functional](../../../../../continuous-linear-functional.md) has a unique representation

$$
\boxed{L(f)=\int_K f\,d\mu,\qquad\|L\|=|\mu|(K).}
$$

Here $|\mu|$ is the [variation measure](../../../../../variation-measure.md); positive functionals correspond exactly to positive regular measures. This is the measure representation theorem, rather than the Hilbert-space representation of a functional by a vector.

For the spectral construction use the convention that the Hilbert [inner product](../../../../../inner-product.md) is linear in its first argument. A unital subalgebra of $\mathcal B(H)$ is understood to contain $I_H$: an algebra whose abstract identity is a smaller projection could not give a resolution normalized by $P(K)=I_H$. On a [compact Hausdorff space](../../../../../compact-hausdorff-space.md), a resolution of the identity is understood to be a normalized regular [projection-valued measure](../../../../../projection-valued-measure.md): its scalar measures are regular, its values are [orthogonal projections](../../../../../orthogonal-projection.md), and it is countably additive in the strong operator topology. Regularity is part of the usual convention needed for the uniqueness assertion; the statement is interpreted in this sense.

The [Commutative Gelfand--Naimark theorem](../../../../../commutative-gelfand-naimark-theorem.md) makes the Gelfand transform an isometric unital star-isomorphism $A\to C(K)$, where $K=\Phi_A$ is compact Hausdorff. Denote its inverse by $\pi:C(K)\to A\subset\mathcal B(H)$. For $x,y\in H$, the [bounded linear functional](../../../../../continuous-linear-functional.md) $f\mapsto\langle\pi(f)x,y\rangle$ has [norm](../../../../../norm.md) at most $\|x\|\|y\|$. Riesz-Markov-Kakutani gives a regular complex measure $\mu_{x,y}$ such that

$$
\langle\pi(f)x,y\rangle=\int_K f\,d\mu_{x,y},\qquad
|\mu_{x,y}|(K)\le\|x\|\|y\|.
$$

Uniqueness makes these measures sesquilinear in $x,y$. For $f\ge0$, the identity $\pi(f)=\pi(\sqrt f)\pi(\sqrt f)^*$ shows positivity, so $\mu_{x,x}$ is positive with total mass $\|x\|^2$.

For every Borel set $B$, the bounded sesquilinear form $(x,y)\mapsto\mu_{x,y}(B)$ determines an operator $P(B)$ by Hilbert-space [Riesz representation theorem](../../../../../riesz-representation-theorem.md), with

$$
\langle P(B)x,y\rangle=\mu_{x,y}(B).
$$

In particular $0\le P(B)\le I$ and $P(B)$ is self-adjoint. We now verify the projection identity rather than assume it.

For continuous $f$, uniqueness of the representing measure applied to continuous test functions gives

$$
\mu_{\pi(f)x,y}=f\mu_{x,y},\qquad
\mu_{x,\pi(\overline f)y}=f\mu_{x,y}.
$$

These identities imply $P(B)\pi(f)=\pi(f)P(B)$. Testing once more against a continuous $g$ gives

$$
\langle\pi(g)P(B)x,y\rangle=\int_B g\,d\mu_{x,y}.
$$

The restriction $1_B\mu_{x,y}$ of a finite regular Borel measure is still regular, so uniqueness in Riesz-Markov-Kakutani yields $\mu_{P(B)x,y}=1_B\mu_{x,y}$. Consequently, for any Borel $C$,

$$
\langle P(C)P(B)x,y\rangle=\mu_{P(B)x,y}(C)
=\mu_{x,y}(B\cap C),\qquad
\boxed{P(C)P(B)=P(B\cap C).}
$$

Taking $C=B$ proves that $P(B)$ is an [orthogonal projection](../../../../../orthogonal-projection.md). Also $P(K)=I$ and $P(\varnothing)=0$. For disjoint $B_j$, these projections are orthogonal, and scalar countable additivity gives weak countable additivity. If $B=\bigcup_j B_j$, then $R_N=P(B)-\sum_{j\le N}P(B_j)$ is the projection of the remaining union and

$$
\|R_Nx\|^2=\mu_{x,x}\left(\bigcup_{j>N}B_j\right)\longrightarrow0.
$$

Thus countable additivity holds in the [strong operator topology](../../../../../strong-operator-topology.md). The scalar measures are the regular measures already constructed. This completes the [scalar-measure construction of a projection-valued measure](../../../../../scalar-measure-construction-of-a-projection-valued-measure.md).

By the integral theorem permitted in the question, continuous $f$ satisfies $\langle(\int f\,dP)x,y\rangle=\int f\,d\mu_{x,y}=\langle\pi(f)x,y\rangle$, and hence $\int f\,dP=\pi(f)$. For $T\in A$, this proves the [spectral theorem for a commutative operator algebra](../../../../../spectral-theorem-for-a-commutative-operator-algebra.md):

$$
\boxed{T=\int_K\widehat T\,dP.}
$$

Any other regular resolution giving these integrals has the same scalar integrals on all of $C(K)$; Riesz-Markov-Kakutani uniqueness forces the same scalar measures and therefore the same projections on every Borel set.

For nonempty open $U\subset K$, compact Hausdorff normality supplies a nonzero [continuous function](../../../../../continuous-function.md) $f$ supported in $U$. If $P(U)=0$, the stated squared-norm identity for spectral integrals gives $\pi(f)=\int f\,dP=0$, contradicting the [isometry](../../../../../isometry.md) of $\pi$. This proves the [full support of a faithful spectral measure](../../../../../full-support-of-a-faithful-spectral-measure.md) property

$$
\boxed{P(U)\ne0\quad\text{for every nonempty open }U\subset K.}
$$

Faithfulness of the representation is essential here.

The [spectral theorem for normal operators](../../../../../spectral-theorem-for-normal-operators.md) says that a bounded [normal operator](../../../../../normal-operator.md) $T$ on a nonzero complex [Hilbert space](../../../../../hilbert-space-split.md) has a unique regular projection-valued measure $E$ on $\sigma(T)$ such that $T=\int z\,dE(z)$. Its support is all of $\sigma(T)$, and bounded Borel functions have the associated [Borel functional calculus for a normal operator](../../../../../borel-functional-calculus-for-a-normal-operator.md).

For the proof sketch, $A=C^*(I,T)$ is commutative because $T$ commutes with $T^*$; polynomials in these two operators commute, as do their [norm](../../../../../norm.md) limits. The map $\Phi_A\to\sigma(T)$, $\varphi\mapsto\varphi(T)$, is onto by the [character of an algebra](../../../../../character-of-an-algebra.md) formula and [spectral permanence for C-star algebras](../../../../../spectral-permanence-for-c-star-algebras.md). It is one-to-one because a [character of an algebra](../../../../../character-of-an-algebra.md) preserves the star operation and its values on $T,T^*$ determine it on their dense polynomial algebra. It is therefore a [homeomorphism](../../../../../homeomorphism.md) from compact $\Phi_A$ to the Hausdorff spectrum. Transport the resolution just constructed through this [homeomorphism](../../../../../homeomorphism.md). It gives the formula for $T$ and full support; conversely a regular resolution for $T$ gives the same integrals for polynomials in $T,T^*$, hence by density the same continuous functional calculus and the same resolution. This argument works without separability of $H$.

Finally choose disjoint nonempty relatively open sets $U,V\subset\sigma(T)$ around two distinct spectral points, and put $Q=E(U)$. Full support gives $Q\ne0$ and $E(V)\ne0$, while $QE(V)=0$, so $Q\ne I$. The spectral integral, or multiplicativity of its Borel calculus with $1_U$, gives $QT=TQ$ and also $QT^*=T^*Q$. Thus $Y=QH$ is closed, nonzero and proper, and $T(Qx)=Q(Tx)\in Y$. The [spectral projection gives a reducing subspace](../../../../../spectral-projection-gives-a-reducing-subspace.md) conclusion is

$$
\boxed{Y=E(U)H\text{ is a nontrivial closed invariant subspace of }T.}
$$

In fact it is a reducing subspace, since it is also invariant under $T^*$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
