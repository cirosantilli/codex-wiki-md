<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [compact Lie group](../../../../../compact-lie-group.md) $G$, the complex [representation ring of a compact group](../../../../../representation-ring-of-a-compact-group.md) $R(G)$ is the [Grothendieck group](../../../../../grothendieck-group.md) of finite-dimensional [continuous](../../../../../continuous-function.md) complex [group representations](../../../../../group-representation.md), with the relations $[M\oplus N]=[M]+[N]$. Multiplication is $[M][N]=[M\otimes N]$, and the unit is the trivial one-dimensional [representation](../../../../../group-representation.md). The ring of [class functions](../../../../../class-function.md) is

$$
c\ell(G)=\{f\in C(G,\mathbb C):f(hgh^{-1})=f(g)
\text{ for all }g,h\in G\},
$$

with pointwise addition and multiplication. The [character](../../../../../character-of-a-representation.md) of $M$ is $\chi_M(g)=\operatorname{tr}\rho_M(g)$. The [trace](../../../../../matrix-trace.md) identities for direct sums and tensor products make

$$
[M]-[N]\longmapsto\chi_M-\chi_N
$$

a well-defined [ring homomorphism](../../../../../ring-homomorphism.md) $\chi:R(G)\to c\ell(G)$.

Normalize [Haar measure](../../../../../haar-measure.md) by $\int_Gdg=1$. Averaging a positive definite [Hermitian inner product](../../../../../hermitian-form.md) gives

$$
(v,w)_G=\int_G(\rho(g)v,\rho(g)w)_0\,dg,
$$

which is positive definite and $G$-invariant. This proves [unitarization of a compact-group representation](../../../../../unitarization-of-a-compact-group-representation.md). In a [unitary representation](../../../../../unitary-representation.md) the [orthogonal complement](../../../../../orthogonal-complement.md) of an [invariant subspace](../../../../../invariant-subspace.md) is invariant. Induction on dimension therefore gives [complete reducibility of compact-group representations](../../../../../complete-reducibility-of-compact-group-representations.md). Hence every element of $R(G)$ is a finite integral linear combination of irreducible classes.

We establish the needed [character orthogonality for compact groups](../../../../../character-orthogonality-for-compact-groups.md) carefully. For irreducible unitary [representations](../../../../../group-representation.md) $V,W$, let $G$ act on $\operatorname{Hom}_{\mathbb C}(W,V)$ by

$$
g\cdot A=\rho_V(g)A\rho_W(g)^{-1}.
$$

Its average $P=\int_G(g\cdot)\,dg$ is a projection onto $\operatorname{Hom}_G(W,V)$: averaging makes every image invariant, and it fixes every intertwiner. The [trace](../../../../../matrix-trace.md) of this action is $\chi_V(g)\overline{\chi_W(g)}$, since the inverse of a unitary [matrix](../../../../../matrix.md) has conjugate [trace](../../../../../matrix-trace.md). Taking the [trace](../../../../../matrix-trace.md) of the projection gives

$$
\int_G\chi_V(g)\overline{\chi_W(g)}\,dg
=\dim\operatorname{Hom}_G(W,V).
$$

For completeness, [Schur's lemma](../../../../../schur-s-lemma.md) follows here from invariance of the kernel and image of an intertwiner. A nonzero intertwiner between irreducibles is an isomorphism. An endomorphism of an irreducible complex [representation](../../../../../group-representation.md) has an [eigenvalue](../../../../../eigenvalue.md) $\lambda$; the noninvertible intertwiner $A-\lambda I$ must vanish. Thus the last dimension is one for isomorphic irreducibles and zero for inequivalent ones.

If a virtual [character](../../../../../character-of-a-representation.md) $\sum_Vn_V\chi_V$ vanishes, integrating it against $\overline{\chi_W}$ gives $n_W=0$ for every irreducible $W$. The irreducible multiplicities therefore distinguish the classes, and

$$
\boxed{\chi:R(G)\longrightarrow c\ell(G)\text{ is injective}.}
$$

This also proves that two finite-dimensional [representations](../../../../../group-representation.md) with the same [character](../../../../../character-of-a-representation.md) are isomorphic.

For [SU(2)](../../../../../su-2-group.md), the irreducibles are $V_k=\operatorname{Sym}^k(\mathbb C^2)$, $k\geq0$, of dimension $k+1$. One can see this classification through the usual $\mathfrak{sl}_2$ operators $H,E,F$: a [highest-weight vector](../../../../../highest-weight-vector.md) $v$ has $Hv=kv$, $Ev=0$, and the relations $[H,E]=2E$, $[H,F]=-2F$, $[E,F]=H$ give, by induction,

$$
EF^jv=j(k-j+1)F^{j-1}v.
$$

The torus weights are integers. If $F^rv\ne0$ but $F^{r+1}v=0$, the identity at $j=r+1$ forces $k=r\geq0$. The vectors $v,Fv,\ldots,F^kv$ span an invariant irreducible module, which in an irreducible [representation](../../../../../group-representation.md) is the whole space. This is the symmetric-power module. Conversely its successive monomial weight vectors are linked by $E,F$ with nonzero coefficients, proving its irreducibility. Thus the [classification of finite-dimensional representations of SU2](../../../../../classification-of-finite-dimensional-representations-of-su2.md) gives every irreducible, rather than just a list of examples.

On the [maximal torus](../../../../../maximal-torus.md) $T=\{\operatorname{diag}(z,z^{-1}):|z|=1\}$, their [characters](../../../../../character-of-a-representation.md) are

$$
\chi_k(z)=z^k+z^{k-2}+\cdots+z^{-k}.
$$

With $x=\chi_1=z+z^{-1}$, multiplication gives $\chi_{k+1}=x\chi_k-\chi_{k-1}$, starting with $\chi_0=1$. Hence each $\chi_k$ is a monic integral polynomial of degree $k$ in $x$. For example $\chi_2=x^2-1$ and $\chi_3=x^3-2x$. They form a basis over $\mathbb Z$, so

$$
\boxed{R(SU(2))\cong\mathbb Z[x],\qquad x=[\mathbb C^2].}
$$

The [character](../../../../../character-of-a-representation.md) map realizes this ring as the finite integral polynomials in $z+z^{-1}$, interpreted as [continuous](../../../../../continuous-function.md) [class functions](../../../../../class-function.md). Its image is not the whole infinite-dimensional ring of [continuous](../../../../../continuous-function.md) [class functions](../../../../../class-function.md); injectivity is the assertion being proved.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
