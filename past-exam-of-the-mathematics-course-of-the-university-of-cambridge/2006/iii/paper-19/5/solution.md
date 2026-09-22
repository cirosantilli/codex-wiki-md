<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Choose the [maximal torus](../../../../../maximal-torus.md) of $SO(2n)$ consisting of rotations in $n$ [orthogonal](../../../../../orthogonal-vectors.md) planes, and write $z_i=e^{i\theta_i}$. In the complexified standard [representation](../../../../../group-representation.md) $E=\mathbb C^{2n}$ the [torus](../../../../../torus.md) [eigenvalues](../../../../../eigenvalue.md) are $z_1,z_1^{-1},\ldots,z_n,z_n^{-1}$, with [weights](../../../../../weight-representation-theory.md) $e_i,-e_i$. For $n\geq2$ the complexified [Lie algebra](../../../../../lie-algebra-split.md) has the [Dn root system](../../../../../dn-root-system.md) $\{\pm e_i\pm e_j:i<j\}$. The [root-space decomposition](../../../../../root-space-decomposition.md) theorem splits this [Lie algebra](../../../../../lie-algebra-split.md) into its [Cartan subalgebra](../../../../../cartan-subalgebra.md) and one-dimensional [root spaces](../../../../../root-space.md). The [Cartan subalgebra](../../../../../cartan-subalgebra.md) contributes the zero [weight](../../../../../weight-representation-theory.md) with multiplicity $n$. Therefore its [character](../../../../../character-of-a-representation.md) is

$$
\boxed{\chi_{\mathrm{ad}}(z)=n+\sum_{i<j}\left(z_i z_j+\frac{z_i}{z_j}+\frac{z_j}{z_i}+\frac1{z_i z_j}\right).}
$$

Take [positive roots](../../../../../positive-root.md) $e_i-e_j,e_i+e_j$ for $i<j$, so $\rho=(n-1,n-2,\ldots,0)$. For $n>2$ the [root](../../../../../root-of-a-root-system.md) $\theta=e_1+e_2$ is a [highest weight](../../../../../highest-weight-of-a-representation.md): its [root vector](../../../../../root-vector.md) is killed by every [positive root](../../../../../positive-root.md) vector, since $\theta+\alpha$ is never a [root](../../../../../root-of-a-root-system.md) for positive $\alpha$. To verify irreducibility without relying on an unstated simplicity theorem, apply complete reducibility and compare [dimensions](../../../../../dimension-vector-space.md). For the [Dn root system](../../../../../dn-root-system.md) the [Weyl dimension formula](../../../../../weyl-dimension-formula.md) reads

$$
\dim V_\lambda=\prod_{i<j}\frac{(\lambda_i+\rho_i)^2-(\lambda_j+\rho_j)^2}{\rho_i^2-\rho_j^2}.
$$

For $\lambda=(1,1,0,\ldots,0)$ only pairs involving the first two indices change. With $s=0,\ldots,n-3$, cancellation gives

$$
\dim V_\theta
=\frac{2n-1}{2n-3}\prod_{s=0}^{n-3}\frac{n^2-s^2}{(n-2)^2-s^2}
=\frac{2n-1}{2n-3}\left(\frac{n(n-1)}2\right)\left(\frac{2(2n-3)}{n-1}\right)
=n(2n-1).
$$

This is exactly $\dim\mathfrak{so}_{2n}(\mathbb C)$, so the [irreducible](../../../../../irreducible-representation.md) summand containing the [highest-weight vector](../../../../../highest-weight-vector.md) exhausts the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md). Thus **for $n>2$ the complexified [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) is [irreducible](../../../../../irreducible-representation.md), with [highest weight](../../../../../highest-weight-of-a-representation.md) $e_1+e_2$**.

For $n=2$, the [roots](../../../../../root-of-a-root-system.md) split into the two independent systems $\{\pm(e_1+e_2)\}$ and $\{\pm(e_1-e_2)\}$. The [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) splits into two [irreducibles](../../../../../irreducible-representation.md) of [dimension](../../../../../dimension-vector-space.md) three, with respective [highest weights](../../../../../highest-weight-of-a-representation.md) $(1,1)$ and $(1,-1)$. Equivalently these are the self-dual and anti-self-dual exterior two-forms in four [dimensions](../../../../../dimension-vector-space.md). Their [characters](../../../../../character-of-a-representation.md) are

$$
1+z_1z_2+(z_1z_2)^{-1},\qquad
1+z_1/z_2+z_2/z_1.
$$

They add to the displayed adjoint [character](../../../../../character-of-a-representation.md). This agrees with the [Chiral decomposition of the complexified so4 Lie algebra](../../../../../chiral-decomposition-of-the-complexified-so4-lie-algebra.md).

For a direct [character](../../../../../character-of-a-representation.md) comparison, put $s(z)=\sum_i(z_i+z_i^{-1})$. The [eigenvalue](../../../../../eigenvalue.md) formula for an [exterior square](../../../../../exterior-square.md) gives

$$
\chi_{\Lambda^2 E}(z)=\frac12\left(s(z)^2-\sum_i(z_i^2+z_i^{-2})\right)
=n+\sum_{i<j}\left(z_i z_j+z_i/z_j+z_j/z_i+(z_i z_j)^{-1}\right).
$$

This is precisely $\chi_{\mathrm{ad}}$. More intrinsically, let $B$ be the nondegenerate [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) preserved by $SO(2n)$ and define

$$
\Psi(u\wedge v)(x)=B(v,x)u-B(u,x)v.
$$

This endomorphism is skew with respect to $B$, so $\Psi$ maps $\Lambda^2E$ to $\mathfrak{so}(E,B)$. In an [orthonormal basis](../../../../../orthonormal-basis.md) the bivectors $e_i\wedge e_j$ map to a basis of skew [skew-symmetric matrices](../../../../../skew-symmetric-matrix.md), proving that it is an [isomorphism](../../../../../isomorphism.md). Since $B$ is invariant,

$$
\Psi(gu\wedge gv)=g\Psi(u\wedge v)g^{-1}.
$$

Thus **the [exterior square](../../../../../exterior-square.md) and the complexified [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) are naturally isomorphic**, explaining the [character](../../../../../character-of-a-representation.md) equality without a [weight](../../../../../weight-representation-theory.md) calculation.

The [symmetric square](../../../../../symmetric-square.md) is not [irreducible](../../../../../irreducible-representation.md). The [inverse metric](../../../../../inverse-metric.md) tensor $\Omega$ is a nonzero invariant vector, and contraction with $B$ splits off its trivial line:

$$
\operatorname{Sym}^2E=\mathbb C\Omega\oplus\operatorname{Sym}^2_0E.
$$

The contraction sends $\Omega$ to $2n$, so this is indeed a [direct sum](../../../../../direct-sum.md). A [highest-weight vector](../../../../../highest-weight-vector.md) $f_1\otimes f_1$, where $f_1$ has [torus](../../../../../torus.md) [weight](../../../../../weight-representation-theory.md) $e_1$, lies in the traceless part because $B(f_1,f_1)=0$, and has [highest weight](../../../../../highest-weight-of-a-representation.md) $2e_1$. The same [dimension](../../../../../dimension-vector-space.md) formula gives, for $n\geq2$,

$$
\dim V_{2e_1}=\prod_{s=0}^{n-2}\frac{(n+1)^2-s^2}{(n-1)^2-s^2}
=\left(\frac{n(n+1)}2\right)\left(\frac{2(2n-1)}n\right)
=(n+1)(2n-1).
$$

This equals $\dim\operatorname{Sym}^2E-1=n(2n+1)-1$. Complete reducibility therefore proves that the traceless part is [irreducible](../../../../../irreducible-representation.md), including the dimension-nine case for $SO(4)$. In particular,

$$
\boxed{\operatorname{Sym}^2(\mathbb C^{2n})\cong\mathbf1\oplus V_{2e_1}\quad(n\geq2),\quad\text{so it is reducible}.}
$$

If the circle case $n=1$ is included, the adjoint [character](../../../../../character-of-a-representation.md) is $1$ and the [symmetric square](../../../../../symmetric-square.md) instead has three one-dimensional [weights](../../../../../weight-representation-theory.md) $2,0,-2$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
