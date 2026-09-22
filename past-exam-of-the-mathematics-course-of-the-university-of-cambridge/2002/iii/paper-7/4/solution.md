<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $K=\sigma(T)$ and use the [continuous functional calculus](../../../../../continuous-functional-calculus.md) $\pi:C(K)\to\mathcal B(H)$. It is a [unital](../../../../../unital-algebra.md) star-homomorphism taking the coordinate function to $T$. This follows from the commutative C-star theorem applied to $C^*(I,T,T^*)$, together with spectral permanence for [C-star subalgebras](../../../../../c-star-subalgebra.md), which is among the permitted C-star results.

Take the [Hilbert space](../../../../../hilbert-space-split.md) inner product linear in its first variable. For a [vector](../../../../../vector.md) $\xi$, let $H_\xi=\overline{\{\pi(f)\xi:f\in C(K)\}}$. This cyclic subspace is invariant under every $\pi(f)$ and its adjoint, so it is reducing. The functional $f\mapsto\langle\pi(f)\xi,\xi\rangle$ is positive because $f\ge0$ implies $\pi(f)=\pi(\sqrt f)^*\pi(\sqrt f)$. It has, by the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md), a finite regular positive [Borel measure](../../../../../borel-measure.md) $\mu_\xi$ on $K$. The identity

$$
\|\pi(f)\xi\|^2=\int_K|f|^2\,d\mu_\xi
$$

makes $f\mapsto\pi(f)\xi$ an [isometry](../../../../../isometry.md) on its quotient by the functions of zero $L^2$ [norm](../../../../../norm.md). Density of [continuous](../../../../../continuous-function.md) functions in $L^2(\mu_\xi)$ extends it to a unitary $U_\xi:L^2(\mu_\xi)\to H_\xi$. Multiplication by a [continuous](../../../../../continuous-function.md) function intertwines with $\pi$ on this subspace.

Choose a maximal family of mutually [orthogonal](../../../../../orthogonal-vectors.md) nonzero cyclic [reducing subspaces](../../../../../reducing-subspace-of-a-hilbert-space-operator.md). Their [orthogonal](../../../../../orthogonal-vectors.md) sum is all of $H$: otherwise its reducing [orthogonal complement](../../../../../orthogonal-complement.md) contains a nonzero [vector](../../../../../vector.md) generating another such subspace. This argument does not require separability. For a bounded [Borel measurable function](../../../../../borel-measurable-function.md) $g$ on $K$, multiplication $M_g$ on every $L^2(\mu_\xi)$ is bounded with [norm](../../../../../norm.md) at most $\|g\|_\infty$. Define on that [orthogonal](../../../../../orthogonal-vectors.md) sum

$$
\boxed{\beta_T(g)=\bigoplus_\xi U_\xi M_gU_\xi^{-1}.}
$$

[Multiplication operators](../../../../../multiplication-operator.md) satisfy $M_{fg}=M_fM_g$, $M_{\overline g}=M_g^*$ and $M_1=I$. The same identities hold for their [direct sums](../../../../../direct-sum.md), and the [norm](../../../../../norm.md) bound is uniform in $\xi$. Thus $\beta_T$ is a norm-decreasing [unital](../../../../../unital-algebra.md) star-homomorphism on the algebra of actual bounded [Borel measurable functions](../../../../../borel-measurable-function.md), and $\beta_T(Z)=T$ because it extends $\pi$. No quotient by a single unspecified measure is being substituted for that Borel algebra.

Choose the bounded Borel measurable square root $s(0)=0$ and $s(z)=|z|^{1/2}e^{i\operatorname{Arg}(z)/2}$ for $z\ne0$, taking $\operatorname{Arg}\in[0,2\pi)$. Let $S=\beta_T(s)$. Then

$$
\boxed{S^2=T,\qquad S^*S=\beta_T(|s|^2)=SS^*.}
$$

Thus every bounded [normal operator](../../../../../normal-operator.md) has a normal square root. The Borel branch is essential in general: on a circle winding about zero a [continuous](../../../../../continuous-function.md) square-root branch need not exist.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
