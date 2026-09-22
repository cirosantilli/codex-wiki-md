<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md) states that every finite-dimensional [Lie algebra representation](../../../../../lie-algebra-representation.md) of a finite-dimensional complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) is a [direct sum](../../../../../direct-sum.md) of [Irreducible Lie algebra representations](../../../../../irreducible-lie-algebra-representation.md). Equivalently, every invariant [vector subspace](../../../../../vector-subspace.md) has an invariant complement.

We use the permitted [Casimir operator](../../../../../casimir-element.md) properties in the following precise form. There is a central quadratic operator $C$ commuting with the action on every module; it is zero on the [trivial Lie algebra representation](../../../../../trivial-lie-algebra-representation.md), and on every nontrivial finite-dimensional [Irreducible Lie algebra representation](../../../../../irreducible-lie-algebra-representation.md) it is a nonzero scalar $c$. This follows from the [Schur lemma](../../../../../schur-s-lemma.md) and the [Casimir eigenvalue](../../../../../casimir-eigenvalue.md) $c_\lambda=(\lambda,\lambda+2\rho)$, using the [Killing form](../../../../../killing-form.md) normalization. We also use the permitted one-dimensional-representation fact: a complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) has only trivial one-dimensional representations. Equivalently, it is a [perfect Lie algebra](../../../../../perfect-lie-algebra.md), $[\mathfrak g,\mathfrak g]=\mathfrak g$, so a character $\mathfrak g\to\mathbb C$ annihilating brackets must vanish. Neither fact assumes complete reducibility of the module being proved reducible.

First prove that every finite-dimensional [short exact sequence](../../../../../short-exact-sequence.md)

$$
0\longrightarrow W\longrightarrow E\longrightarrow\mathbb C\longrightarrow0
$$

with trivial quotient splits. If $W$ is nontrivial irreducible, the [Casimir operator](../../../../../casimir-element.md) $C_E$ has image in $W$ and restricts to $cI_W$ there. Consequently $\ker C_E$ is a one-dimensional invariant complement to $W$. If $W$ is trivial irreducible, $E$ has a [basis](../../../../../basis.md) in which every action is $\begin{pmatrix}0&a(x)\\0&0\end{pmatrix}$. The [Lie algebra representation](../../../../../lie-algebra-representation.md) identity makes $a([x,y])=0$, so the one-dimensional-representation fact gives $a=0$ and again the sequence splits.

For general $W$, induct on $\dim W$. Choose an irreducible submodule $W_1\subseteq W$. The induced sequence with kernel $W/W_1$ and middle term $E/W_1$ splits by induction. The inverse image $E_1\subseteq E$ of its invariant complement is a submodule fitting into $0\to W_1\to E_1\to\mathbb C\to0$. The irreducible-kernel case gives an invariant line in $E_1$ mapping isomorphically to the quotient. It is also an invariant complement to $W$ in $E$. The case $W=0$ starts this induction. This proves [splitting of a trivial quotient for a semisimple Lie algebra](../../../../../casimir-splitting-of-a-trivial-quotient.md), including kernels that are not assumed completely reducible.

Now let $U\subseteq V$ be any [invariant subspace](../../../../../invariant-subspace.md). On the [Hom representation](../../../../../hom-representation.md) $\operatorname{Hom}(V,U)$ the action is

$$
(x\cdot T)(v)=x\cdot T(v)-T(x\cdot v).
$$

Let $E$ consist of the maps whose restriction to $U$ is a scalar multiple of $I_U$. This is a submodule, and restriction gives

$$
0\longrightarrow\operatorname{Hom}(V/U,U)\longrightarrow E\longrightarrow\mathbb C\longrightarrow0.
$$

The right-hand map is surjective because an ordinary [linear projection](../../../../../projection-linear-algebra.md) $V\to U$ exists; its quotient action is trivial because a commutator with $I_U$ is zero. The splitting just proved supplies an invariant $T\in E$ with $T|_U=I_U$. Thus $T$ intertwines the actions, $T^2=T$, and

$$
\boxed{V=U\oplus\ker T\quad\text{as }\mathfrak g\text{-modules}.}
$$

The cases $U=0$ and $U=V$ are immediate. Choosing an irreducible submodule and repeating this complement construction proves the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md). This last step is [invariant complement from an equivariant projection](../../../../../invariant-complement-from-an-equivariant-projection.md).

Dropping finite dimensionality gives an example with the complex [simple Lie algebra](../../../../../simple-lie-algebra.md) $\mathfrak{sl}_2$. Its [Verma module](../../../../../verma-module.md) of [highest weight](../../../../../highest-weight-of-a-representation.md) zero has a [basis](../../../../../basis.md) $v_0,v_1,\ldots$ with

$$
fv_k=v_{k+1},\qquad hv_k=-2kv_k,\qquad ev_k=k(1-k)v_{k-1},
$$

where $ev_0=0$. These actions obey $[h,e]=2e$, $[h,f]=-2f$, $[e,f]=h$. The span of $v_1,v_2,\ldots$ is a proper submodule and the quotient is trivial. It has no invariant complement: such a complement would be a trivial line, while $f$ is injective on the entire module. Thus **a simple Lie algebra can have an infinite-dimensional representation that is not completely reducible**, even over $\mathbb C$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
