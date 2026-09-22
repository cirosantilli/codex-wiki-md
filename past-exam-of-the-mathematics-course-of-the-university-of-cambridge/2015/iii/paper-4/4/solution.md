<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use homological grading $d_n:C_n\to C_{n-1}$, with zero terms below degree zero. In the [projective model structure on nonnegative chain complexes](../../../../../projective-model-structure-on-nonnegative-chain-complexes.md), the classes are:

- [Model weak equivalences](../../../../../model-weak-equivalence.md) are [quasi-isomorphisms](../../../../../quasi-isomorphism.md), inducing isomorphisms on every $H_n$.
- [Model fibrations](../../../../../model-fibration.md) are maps surjective in every strictly positive degree $n\geq1$; surjectivity in degree zero is not part of this definition.
- [Model cofibrations](../../../../../model-cofibration.md) are degreewise injections with projective cokernel in every degree. The underlying module injections then split degreewise, although these splittings need not commute with the differential.

Thus a cofibrant complex has a projective module in each degree, and every object is fibrant. An [projective acyclic fibration](../../../../../acyclic-fibration-in-the-projective-chain-complex-model-structure.md) is equivalently a degreewise surjective [quasi-isomorphism](../../../../../quasi-isomorphism.md), including degree zero. To see the degree-zero assertion, lift a degree-zero homology class using the homology isomorphism, then lift the boundary discrepancy using surjectivity in degree one. Conversely a degreewise surjective [quasi-isomorphism](../../../../../quasi-isomorphism.md) has the requisite positive-degree surjections.

Let $S^n(R)$ be the [sphere chain complex](../../../../../sphere-chain-complex.md) with $R$ in degree $n$ and zero elsewhere. Let $D^n(R)$, for $n\geq1$, be the [disk chain complex](../../../../../disk-chain-complex.md) with $R$ in degrees $n,n-1$ and identity differential. The [generating cofibrations for nonnegative chain complexes](../../../../../generating-cofibrations-for-nonnegative-chain-complexes.md) are

$$
\boxed{I=\{0\to S^0(R)\}\ \cup\ \{S^{n-1}(R)\hookrightarrow D^n(R):n\geq1\}.}
$$

Each is a [model cofibration](../../../../../model-cofibration.md): its degreewise cokernel is a copy of $R$ in one degree. The extra degree-zero generator must not be omitted.

Here is the [lifting characterization of an acyclic chain-complex fibration](../../../../../lifting-characterization-of-an-acyclic-chain-complex-fibration.md). A [right lifting property](../../../../../right-lifting-property.md) for $S^{n-1}(R)\to D^n(R)$ says that whenever $x\in Z_{n-1}X$ and $y\in Y_n$ satisfy $f(x)=dy$, there is $z\in X_n$ with $dz=x$ and $f(z)=y$. The generator $0\to S^0(R)$ says that $f_0$ is surjective. For a degreewise surjective [quasi-isomorphism](../../../../../quasi-isomorphism.md), its kernel is acyclic by the [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md). Choose a preliminary lift $z_0$ of $y$. Then $dz_0-x$ is a cycle in the kernel; subtract an element of the kernel whose boundary is this cycle. This gives the required $z$.

Conversely the lifting conditions make the kernel acyclic: take $y=0$ and any kernel cycle $x$. They also imply degreewise surjectivity inductively. Having surjectivity below degree $n$, lift $dy$ to an element of $X_{n-1}$, correct its boundary within the acyclic kernel to make it a cycle, and apply the lifting condition to lift $y$. For $n=1$ the chosen degree-zero element is already a cycle. A degreewise surjective map with acyclic kernel is a [quasi-isomorphism](../../../../../quasi-isomorphism.md) by the [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md). Hence **$I$-injectives are exactly acyclic fibrations**.

An object $A$ is [sequentially small](../../../../../sequentially-small-object.md) if for every sequential diagram $Z_0\to Z_1\to\cdots$, the natural map

$$
\boxed{\operatorname*{colim}_k\operatorname{Hom}(A,Z_k)\ \longrightarrow\ \operatorname{Hom}\left(A,\operatorname*{colim}_k Z_k\right)}
$$

is bijective. Surjectivity says that a map out of $A$ factors through a finite stage; injectivity says that two such maps agreeing in the colimit agree at a later finite stage. The relative version restricts to the stated class of sequential diagrams. The domains in $I$ have this property: maps from $S^{n-1}(R)$ are cycles in one degree, and [filtered colimits](../../../../../filtered-colimit-of-modules.md) commute with these finite equations. Their sequential smallness is also permitted by the hint.

Apply the [small object argument](../../../../../small-object-argument.md) to the map $a:X\to Y$. Put $Z_0=X$, $p_0=a$. Given $p_k:Z_k\to Y$, take the set of all commutative squares with a generator $i:A_i\to B_i$ on the left and $p_k$ on the right. Form the [pushout](../../../../../pushout.md) of the coproduct of all these $i$ along their maps into $Z_k$, obtaining $Z_{k+1}$. Each bottom map $B_i\to Y$ induces the compatible map $p_{k+1}:Z_{k+1}\to Y$. Repeat for all $k\geq0$, and set $Z_\infty=\operatorname*{colim}_k Z_k$. This gives

$$
\boxed{X\xrightarrow{j}Z_\infty\xrightarrow{p}Y,\qquad pj=a.}
$$

Concretely, attaching $S^{n-1}(R)\to D^n(R)$ adds a free generator in degree $n$ whose boundary is the chosen existing cycle; attaching $0\to S^0(R)$ adds a free degree-zero generator. Thus $j$ is an injection, and its cokernel in each degree is free on the newly attached generators. It is therefore a [model cofibration](../../../../../model-cofibration.md); this also illustrates the [relative cell complex](../../../../../relative-cell-complex.md) description of the left factor.

For a lifting square into $Z_\infty\to Y$, sequential smallness of its domain $A_i$ factors the top map through some $Z_k$. The commutativity is already an equality in $Y$, so this is one of the squares attached at stage $k+1$. Its new cell supplies a lift $B_i\to Z_{k+1}\to Z_\infty$. Hence $p$ has the [right lifting property](../../../../../right-lifting-property.md) with respect to every element of $I$, and is an [projective acyclic fibration](../../../../../acyclic-fibration-in-the-projective-chain-complex-model-structure.md). **Every map has the required cofibration–acyclic-fibration factorization.** Only the domains need sequential smallness; there is no requirement that $X$, $Y$ or the coproduct of all cells be small.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
