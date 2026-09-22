<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [unipotent algebraic group](../../../../../unipotent-algebraic-group.md) admits a faithful linear representation in which every group element is a [unipotent matrix](../../../../../unipotent-matrix.md). For $E=\operatorname{End}_Q(X)$, invertibility is the nonvanishing condition $\prod_i\det h_i\ne0$. Therefore $\operatorname{Aut}_Q(X)=E^\times$ is a nonempty [Zariski-open subset](../../../../../zariski-open-set.md) of the vector space $E$.

Take a [Krull-Schmidt decomposition](../../../../../krull-schmidt-decomposition.md) $X\cong\bigoplus_{a=1}^rM_a^{\oplus m_a}$, with pairwise nonisomorphic [indecomposable modules](../../../../../indecomposable-module.md). The [Fitting lemma](../../../../../fitting-lemma.md) makes each $\operatorname{End}_Q(M_a)$ a [local endomorphism ring](../../../../../local-endomorphism-ring.md). Its residue [division algebra](../../../../../division-algebra.md) is $k$: over an [algebraically closed field](../../../../../algebraically-closed-field.md), every element of a finite-dimensional division algebra has an eigenvalue and hence must be scalar. The [semisimple quotient of a module endomorphism algebra](../../../../../semisimple-quotient-of-a-module-endomorphism-algebra.md) consequently gives, for the [Jacobson radical](../../../../../jacobson-radical.md) $J=J(E)$,

$$
E/J\cong\prod_{a=1}^rM_{m_a}(k),\qquad E^\times\longrightarrow\prod_{a=1}^r\operatorname{GL}_{m_a}(k)
$$

is surjective with kernel $1+J$. The nilpotence of $J$ makes $(1+j)^{-1}=1-j+j^2-\cdots$ finite and each $1+j$ unipotent. The kernel is closed and normal. Acting on the multiplicity spaces embeds the product of [general linear groups](../../../../../general-linear-group.md) back into $E^\times$ and splits this quotient. This proves the [Levi decomposition of a quiver automorphism group](../../../../../levi-decomposition-of-a-quiver-automorphism-group.md)

$$
\boxed{\operatorname{Aut}_Q(X)\cong(1+J)\rtimes\prod_{a=1}^r\operatorname{GL}_{m_a}(k)}.
$$

Since $1+J$ is the [unipotent radical](../../../../../unipotent-radical.md), a nonzero $X$ is indecomposable exactly when **$\operatorname{Aut}_Q(X)/R_u(\operatorname{Aut}_Q(X))\cong\mathbb G_m$**: the product has a single factor of size one.

For the [base change action on quiver representations](../../../../../base-change-action-on-quiver-representations.md), the orbit map is $g\mapsto(g_jx_\rho g_i^{-1})_{\rho:i\to j}$. Substituting $g_i=I+\epsilon u_i$, with $\epsilon^2=0$, shows its differential is

$$
\boxed{\xi_x(u)_\rho=u_jx_\rho-x_\rho u_i}.
$$

Its kernel is $\operatorname{End}_Q(X)$. The stabilizer is smooth because it is open in that vector space. Hence the differential has rank $\dim\operatorname{GL}(\mathbf n)-\dim\operatorname{Aut}_Q(X)=\dim\mathcal O_X$, and its image is the [Zariski tangent space](../../../../../zariski-tangent-space.md) $T_x\mathcal O_X$. The [normal space to a quiver orbit](../../../../../normal-space-to-a-quiver-orbit.md) is therefore

$$
\boxed{T_x\operatorname{Rep}_Q(\mathbf n)/T_x\mathcal O_X\cong\operatorname{Ext}^1_Q(X,X)}.
$$

The ambient [quiver representation space](../../../../../quiver-representation-space.md) is an irreducible affine space, and orbits are locally closed. An orbit is open exactly when its dimension equals that ambient dimension, equivalently when $\operatorname{Ext}^1_Q(X,X)=0$. This proves that [rigid quiver representations have open orbits](../../../../../rigid-quiver-representations-have-open-orbits.md). Such an orbit is dense and unique, since two nonempty open subsets of an irreducible space intersect.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
