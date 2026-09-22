<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [symplectic manifold](../../../../../symplectic-manifold.md) is a smooth manifold $P$ with a closed, nondegenerate [two-form](../../../../../2-form.md) $\omega$. Nondegeneracy forces $\dim P=2n$. Examples are $\mathbb R^{2n}$ with $\omega=\sum_i dq^i\wedge dp_i$, an oriented surface with a nowhere-zero area form, and every [cotangent bundle](../../../../../cotangent-bundle.md) with its canonical form.

A [Poisson manifold](../../../../../poisson-manifold.md) has a bivector $\Pi$ such that $\{f,g\}=\Pi(df,dg)$ is an antisymmetric bilinear [Poisson bracket](../../../../../poisson-bracket.md), is a derivation in each argument, and satisfies the [Jacobi identity](../../../../../jacobi-identity.md). Its rank need not be full or constant. The zero bivector gives a [Poisson manifold](../../../../../poisson-manifold.md) on any smooth manifold, including an odd-dimensional or nonorientable one. A nonzero example on $\mathbb R^3$ is the [Lie-Poisson bracket](../../../../../lie-poisson-bracket.md) $\{x_i,x_j\}=\epsilon_{ijk}x_k$: it has rank two off the origin and rank zero at the origin, so it does not arise from a [symplectic form](../../../../../symplectic-form.md) on the whole three-dimensional space. Even on $\mathbb R^2$, $\Pi=x\partial_x\wedge\partial_y$ is Poisson, since its Jacobi condition is a three-vector and hence vanishes, but its degeneracy on $x=0$ prevents it from being the inverse of a global [symplectic form](../../../../../symplectic-form.md). A manifold carrying a degenerate Poisson structure might separately admit some other symplectic structure; these are distinct claims.

At each point of a [symplectic manifold](../../../../../symplectic-manifold.md), linear nondegeneracy gives a basis with $\omega=\sum_i e^i\wedge f^i$. Its top [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md) is

$$
\frac{\omega^n}{n!}=e^1\wedge f^1\wedge\cdots\wedge e^n\wedge f^n\ne0.
$$

Thus $\omega^n/n!$ is a global nowhere-zero [volume form](../../../../../volume-form.md) and selects a consistent [symplectic orientation](../../../../../symplectic-orientation.md). This proves **every symplectic manifold is orientable** without choosing a global frame.

Let $\pi:T^*M\to M$ and let a point of the [cotangent bundle](../../../../../cotangent-bundle.md) be $(x,p)$ with $p\in T_x^*M$. Define the canonical [Liouville one-form](../../../../../canonical-one-form-on-a-cotangent-bundle.md) intrinsically by $\theta_{(x,p)}(V)=p(d\pi(V))$. In local coordinates it is $\theta=p_i dq^i$, so

$$
\omega=-d\theta=dq^i\wedge dp_i.
$$

This definition is global, $d\omega=0$ by $d^2=0$, and its coordinate matrix has invertible blocks. Hence **$T^*M$ is symplectic for every smooth $M$**, even if $M$ itself is not orientable.

The [coordinate Jacobi condition for a Poisson bivector](../../../../../coordinate-jacobi-condition-for-a-poisson-bivector.md) is

$$
\boxed{\Pi^{i\ell}\partial_\ell\Pi^{jk}+\Pi^{j\ell}\partial_\ell\Pi^{ki}+\Pi^{k\ell}\partial_\ell\Pi^{ij}=0.}
$$

Necessity follows by applying the [Jacobi identity](../../../../../jacobi-identity.md) to three coordinate functions. For arbitrary functions, the second-derivative terms in the Jacobiator cancel by antisymmetry of $\Pi$; the terms left are exactly this coefficient multiplying $f_i g_j h_k$, proving sufficiency.

For a [symplectic form](../../../../../symplectic-form.md), take $\iota_{X_f}\omega=df$ and $\{f,g\}=\omega(X_f,X_g)$. With these signs the matrix of $\Pi$ is $-\omega^{-1}$. Differentiation gives $\partial_\ell\Pi=\Pi(\partial_\ell\omega)\Pi$. The cyclic expression above consequently equals

$$
-\Pi^{ia}\Pi^{jb}\Pi^{kc}(\partial_a\omega_{bc}+\partial_b\omega_{ca}+\partial_c\omega_{ab}),
$$

which vanishes because $d\omega=0$. This directly proves that a [symplectic manifold](../../../../../symplectic-manifold.md) defines a [Poisson manifold](../../../../../poisson-manifold.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
