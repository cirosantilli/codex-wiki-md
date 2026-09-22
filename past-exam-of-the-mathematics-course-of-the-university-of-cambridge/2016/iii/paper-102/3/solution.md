<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Schur's lemma says that a nonzero intertwiner between irreducible representations is an isomorphism; over $\mathbb C$, every endomorphism of a finite-dimensional irreducible representation is scalar.** To prove the [Schur lemma](../../../../../schur-s-lemma.md), let $T:V\to W$ be a [intertwining operator](../../../../../intertwining-operator.md) between [irreducible representations](../../../../../irreducible-representation.md). Its [kernel](../../../../../kernel-of-a-linear-map.md) and [image of a linear map](../../../../../image-of-a-linear-map.md) are invariant. If $T\ne0$, irreducibility forces $\ker T=0$ and $\operatorname{im}T=W$. This proves the first assertion over any field. In particular the endomorphisms of an [irreducible representation](../../../../../irreducible-representation.md) form a [division ring](../../../../../division-ring.md).

When $V$ is finite-dimensional over an [algebraically closed field](../../../../../algebraically-closed-field.md), an endomorphism $T$ has an [eigenvalue](../../../../../eigenvalue.md) $\lambda$. The endomorphism $T-\lambda I$ has nonzero [kernel](../../../../../kernel-of-a-linear-map.md). By the first assertion it must be zero, so $T=\lambda I$. Consequently, for complex finite-dimensional [irreducible representations](../../../../../irreducible-representation.md), the space of [intertwining operators](../../../../../intertwining-operator.md) has dimension zero for nonisomorphic representations and dimension one for isomorphic representations.

**Every finite-dimensional representation of a complex semisimple Lie algebra is completely reducible.** We prove the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md) using the allowed [Casimir operator](../../../../../casimir-element.md) facts, without assuming a splitting in advance. For dual [bases](../../../../../basis.md) $x_i,x^i$ with respect to the [Killing form](../../../../../killing-form.md), the [Casimir element](../../../../../casimir-element.md)

$$
\Omega=\sum_i x_i x^i\in U(\mathfrak g)
$$

is central in the [universal enveloping algebra](../../../../../universal-enveloping-algebra.md). Hence its [Casimir operator](../../../../../casimir-element.md) $C_M=\sum_i\rho_M(x_i)\rho_M(x^i)$ commutes with the action on every [Lie algebra representation](../../../../../lie-algebra-representation.md) $M$ and is compatible with [subrepresentations](../../../../../subrepresentation.md), [quotient representations](../../../../../quotient-representation.md), and [intertwining operators](../../../../../intertwining-operator.md). On the [trivial Lie algebra representation](../../../../../trivial-lie-algebra-representation.md) it acts by zero. On every nontrivial finite-dimensional [Irreducible Lie algebra representation](../../../../../irreducible-lie-algebra-representation.md) it acts by a nonzero scalar.

For clarity, the last fact can be expressed by the [Casimir eigenvalue](../../../../../casimir-eigenvalue.md) formula: on an irreducible with [dominant integral weight](../../../../../dominant-integral-weight.md) $\lambda$, the scalar is $(\lambda,\lambda+2\rho)$, with the inner product induced by the [Killing form](../../../../../killing-form.md) and $\rho$ the [half-sum of positive roots](../../../../../half-sum-of-positive-roots.md). On the real span of the [weights](../../../../../weight-representation-theory.md) this inner product is positive definite, and the scalar is positive for $\lambda\ne0$. For a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) with several simple factors the scalars add, so a nontrivial representation still gives a nonzero scalar. These are properties of the [Casimir operator](../../../../../casimir-element.md) being used here.

First establish [Casimir splitting of a trivial quotient](../../../../../casimir-splitting-of-a-trivial-quotient.md). Suppose

$$
0\longrightarrow N\longrightarrow E\overset{q}{\longrightarrow}\mathbb C\longrightarrow0
$$

is a [short exact sequence](../../../../../short-exact-sequence.md) of finite-dimensional [Lie algebra representations](../../../../../lie-algebra-representation.md), with trivial quotient. The [generalized eigenspaces](../../../../../generalized-eigenspace.md) of $C_E$ are invariant, so

$$
E=E_0\oplus\bigoplus_{c\ne0}E_c.
$$

Each $E_c$ with $c\ne0$ maps to zero under $q$: applying a sufficiently large power of $C_E-cI$ and using $C_{\mathbb C}=0$ gives $(-c)^r q(e)=0$. Thus $q(E_0)=\mathbb C$.

Take a [composition series of a module](../../../../../composition-series-of-a-module.md) of $E_0$. The [Casimir operator](../../../../../casimir-element.md) is nilpotent on $E_0$, so its scalar on every irreducible [composition factor](../../../../../composition-factor.md) is zero. The stated [Casimir operator](../../../../../casimir-element.md) property makes every such factor trivial. In a [basis](../../../../../basis.md) adapted to the [composition series of a module](../../../../../composition-series-of-a-module.md), the image of $\mathfrak g$ on $E_0$ therefore consists of strictly upper triangular [matrices](../../../../../matrix.md), so that image is [solvable](../../../../../solvable-lie-algebra.md). The allowed fact that a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) acts trivially on every one-dimensional representation implies that $\mathfrak g$ is a [perfect Lie algebra](../../../../../perfect-lie-algebra.md): otherwise a nonzero [linear functional](../../../../../linear-functional.md) on $\mathfrak g/[\mathfrak g,\mathfrak g]$ would define a nontrivial one-dimensional [Lie algebra representation](../../../../../lie-algebra-representation.md). Thus $\mathfrak g=[\mathfrak g,\mathfrak g]$, and its image is consequently a [perfect Lie algebra](../../../../../perfect-lie-algebra.md) too. A [perfect Lie algebra](../../../../../perfect-lie-algebra.md) that is also a [solvable Lie algebra](../../../../../solvable-lie-algebra.md) is zero, since its [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md) is constant until it vanishes. Hence $\mathfrak g$ acts trivially on $E_0$. Choose $e\in E_0$ with $q(e)=1$. The map $1\mapsto e$ is an invariant section, proving the [split short exact sequence](../../../../../split-short-exact-sequence.md) assertion.

Now let $W\subseteq V$ be any nonzero [subrepresentation](../../../../../subrepresentation.md). On the [Hom representation](../../../../../hom-representation.md) $\operatorname{Hom}(V,W)$ the action is

$$
(x\cdot f)(v)=x f(v)-f(xv).
$$

Consider the invariant subspace

$$
E=\{f\in\operatorname{Hom}(V,W):f|_W\in\mathbb C I_W\}.
$$

Restriction produces a [short exact sequence](../../../../../short-exact-sequence.md)

$$
0\longrightarrow\operatorname{Hom}(V/W,W)\longrightarrow E\longrightarrow\mathbb C I_W\longrightarrow0.
$$

Surjectivity follows by extending $I_W$ to a linear map on $V$. The quotient is trivial, because $I_W$ commutes with the action on $W$. The preceding [Casimir splitting of a trivial quotient](../../../../../casimir-splitting-of-a-trivial-quotient.md) yields an invariant $p:V\to W$ with $p|_W=I_W$. Thus

$$
V=W\oplus\ker p,
$$

and $\ker p$ is invariant. The zero [subrepresentation](../../../../../subrepresentation.md) also has a complement. Repeatedly splitting off an irreducible [subrepresentation](../../../../../subrepresentation.md) now gives a [direct sum](../../../../../direct-sum.md) of irreducibles, proving the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md).

A [derivation of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md) is a linear map $D:\mathfrak g\to\mathfrak g$ satisfying the [Leibniz rule](../../../../../leibniz-rule.md)

$$
D[x,y]=[Dx,y]+[x,Dy].
$$

The space $\operatorname{Der}(\mathfrak g)$ is a [vector subspace](../../../../../vector-subspace.md) of $\operatorname{End}(\mathfrak g)$. Equip it with the [commutator](../../../../../commutator.md) $[D,E]=DE-ED$. Expanding the [Leibniz rule](../../../../../leibniz-rule.md) twice gives

$$
\begin{aligned}
DE[x,y]&=[DEx,y]+[Ex,Dy]+[Dx,Ey]+[x,DEy],\\
ED[x,y]&=[EDx,y]+[Dx,Ey]+[Ex,Dy]+[x,EDy].
\end{aligned}
$$

Subtracting proves that $[D,E]$ is again a [derivation of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md). Antisymmetry and the [Jacobi identity](../../../../../jacobi-identity.md) hold for the [commutator](../../../../../commutator.md) in every associative endomorphism algebra, so this defines the [derivation Lie algebra](../../../../../derivation-lie-algebra.md).

The [Jacobi identity](../../../../../jacobi-identity.md) says that $\operatorname{ad}x$ is a [derivation of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md). Moreover, for $D\in\operatorname{Der}(\mathfrak g)$,

$$
[D,\operatorname{ad}x](y)=D[x,y]-[x,Dy]=[Dx,y],
$$

so

$$
\boxed{[D,\operatorname{ad}x]=\operatorname{ad}(Dx).}
$$

This makes $\operatorname{ad}\mathfrak g$ an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) in $\operatorname{Der}(\mathfrak g)$.

Finally suppose $\mathfrak g$ is [semisimple](../../../../../semisimple-lie-algebra-split.md). Let $\mathfrak g$ act on $\operatorname{Der}(\mathfrak g)$ by $x\cdot D=[\operatorname{ad}x,D]$. The [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md) supplies an invariant complement $M$ to $\operatorname{ad}\mathfrak g$. For $D\in M$, invariance gives $[\operatorname{ad}x,D]\in M$, while the [ideal](../../../../../ideal.md) identity above gives $[\operatorname{ad}x,D]\in\operatorname{ad}\mathfrak g$. Their intersection is zero, so $\operatorname{ad}(Dx)=0$ for every $x$. The [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md) of a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) is zero, hence $Dx=0$ for every $x$, and $M=0$. Therefore

$$
\boxed{\operatorname{Der}(\mathfrak g)=\operatorname{ad}\mathfrak g.}
$$

Every [derivation of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md) is inner, and the element giving it is unique because the [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md) vanishes.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
