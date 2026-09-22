<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a complex finite-dimensional [simple Lie algebra](../../../../../simple-lie-algebra.md), a [Cartan subalgebra](../../../../../cartan-subalgebra.md) $\mathfrak h$ is a maximal commuting subalgebra of elements whose adjoint maps are semisimple. Equivalently in this setting it is a nilpotent self-normalizing subalgebra. Its dimension is the [rank of a semisimple Lie algebra](../../../../../rank-of-a-semisimple-lie-algebra.md). Simultaneous diagonalization of its [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) gives the [root-space decomposition](../../../../../root-space-decomposition.md)

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}\mathfrak g_\alpha,\qquad \mathfrak g_\alpha=\{E:[H,E]=\alpha(H)E\text{ for all }H\in\mathfrak h\}.
$$

A [root of a root system](../../../../../root-of-a-root-system.md) is a nonzero linear functional $\alpha$ for which this [root space](../../../../../root-space.md) is nonzero. For a complex semisimple algebra each [root space](../../../../../root-space.md) is one-dimensional. A [Cartan-Weyl basis](../../../../../cartan-weyl-basis.md) consists of a basis $H_i$ of $\mathfrak h$ and one nonzero [root vector](../../../../../root-vector.md) $E_\alpha$ for every root.

The general [Lie brackets](../../../../../lie-bracket.md) have the form

$$
[H_i,H_j]=0,\qquad[H_i,E_\alpha]=\alpha(H_i)E_\alpha,
$$



$$
[E_\alpha,E_\beta]=\begin{cases}N_{\alpha\beta}E_{\alpha+\beta},&\alpha+\beta\in\Phi,\\\text{an element of }\mathfrak h,&\beta=-\alpha,\\0,&\alpha+\beta\notin\Phi\cup\{0\}.\end{cases}
$$

For the opposite-root bracket, use the [Killing form](../../../../../killing-form.md) to define $h_\alpha$ by $\kappa(h_\alpha,H)=\alpha(H)$. Its [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md) property gives

$$
[E_\alpha,E_{-\alpha}]=\kappa(E_\alpha,E_{-\alpha})h_\alpha.
$$

One may normalize the [root vectors](../../../../../root-vector.md) so that the pairing is one. If instead one uses a [coroot](../../../../../coroot.md) as the opposite-root bracket, the root-vector normalization changes accordingly. In particular, root evaluation coordinates cannot simply be used as coefficients in a nonorthonormal Cartan basis.

For the matrix calculation take $N\ge2$. The [complexification of a Lie algebra](../../../../../complexification-of-a-lie-algebra.md) of the [special unitary group](../../../../../special-unitary-group.md) [Lie algebra](../../../../../lie-algebra-split.md) is the [special linear Lie algebra](../../../../../special-linear-lie-algebra.md) $\mathfrak{sl}_N(\mathbb C)$: traceless complex matrices. Its [Cartan subalgebra](../../../../../cartan-subalgebra.md) consists of traceless diagonal matrices. Write $E_{jk}=\mathcal T^{(j,k)}$ for the [matrix units](../../../../../matrix-unit.md). The given Cartan basis is $H_i=E_{ii}-E_{i+1,i+1}$, $1\le i<N$, and the other basis elements are $E_{jk}$ with $j\ne k$.

The matrix-unit identity $E_{jk}E_{lm}=\delta_{kl}E_{jm}$ gives

$$
[H_i,E_{jk}]=\left(\delta_{ij}-\delta_{i+1,j}-\delta_{ik}+\delta_{i+1,k}\right)E_{jk}.
$$

Thus all the roots, expressed as evaluation vectors in this precise Cartan basis, are

$$
\boxed{(\alpha_{jk})_i=\alpha_{jk}(H_i)=\delta_{ij}-\delta_{i+1,j}-\delta_{ik}+\delta_{i+1,k},\quad j\ne k,\quad 1\le i<N.}
$$

They are the functionals $e_j-e_k$ on traceless diagonal matrices; there are $N(N-1)$ of them. The corresponding [root vector](../../../../../root-vector.md) is $E_{jk}$. Together with $N-1$ Cartan generators, they give $N^2-1$ basis elements. The [simple roots](../../../../../simple-root.md) can be chosen as $\alpha_{i,i+1}$, whose evaluation vectors are the rows of the type-$A_{N-1}$ [Cartan matrix](../../../../../cartan-matrix.md), with $2$ on the diagonal and $-1$ on adjacent entries. These vectors are evaluations on $H_i$, not coordinates in an orthonormal realization of the [root system](../../../../../root-system.md).

To express every bracket strictly in the chosen basis, introduce the abbreviation

$$
D_{jk}=E_{jj}-E_{kk}=\begin{cases}\displaystyle\sum_{p=j}^{k-1}H_p,&j<k,\\\displaystyle-\sum_{p=k}^{j-1}H_p,&j>k.\end{cases}
$$

Then all pairs are covered by

$$
\boxed{[H_i,H_l]=0,\qquad[H_i,E_{jk}]=(\alpha_{jk})_iE_{jk},}
$$



$$
\boxed{[E_{jk},E_{lm}]=\begin{cases}D_{jk},&k=l,\ j=m,\\E_{jm},&k=l,\ j\ne m,\\-E_{lk},&j=m,\ k\ne l,\\0,&k\ne l,\ j\ne m.\end{cases}}
$$

Here both input [root vectors](../../../../../root-vector.md) have distinct row and column indices. The first case is the only one producing diagonal [matrix units](../../../../../matrix-unit.md), and the displayed sum of $H_p$ resolves them completely into the chosen Cartan basis. Reversing the order gives the negative bracket. This also shows explicitly that the two nonzero non-Cartan cases have [structure constants](../../../../../structure-constant.md) $+1$ and $-1$, and verifies the required root-addition rule.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
