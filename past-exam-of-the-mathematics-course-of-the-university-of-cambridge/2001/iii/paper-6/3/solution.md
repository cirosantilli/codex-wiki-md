<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\mathcal F=C(X,[0,1])$. Form the evaluation map into a [product space](../../../../../product-space.md)

$$
e:X\longrightarrow[0,1]^{\mathcal F},\qquad e(x)=(f(x))_{f\in\mathcal F},\qquad \beta X=\overline{e(X)}.
$$

The cube is [compact](../../../../../compact-space.md) by [Tychonoff's theorem](../../../../../tychonoff-s-theorem.md) and [Hausdorff](../../../../../hausdorff-space.md), so its closed subspace $\beta X$ is a [compact Hausdorff space](../../../../../compact-hausdorff-space.md). A [completely regular Hausdorff space](../../../../../completely-regular-hausdorff-space.md) has enough [continuous functions](../../../../../continuous-function.md) to separate points and closed sets. Consequently $e$ is injective and continuous, and is a [topological embedding](../../../../../topological-embedding.md): given $x\in O$ open, choose $f$ with $f(x)=0$ and $f=1$ off $O$; the coordinate neighborhood $f<1/2$ pulls back to a neighborhood of $x$ inside $O$. Identify $X$ with this dense embedded subspace. This constructs the [Stone-Čech compactification](../../../../../stone-cech-compactification.md).

Each $f\in\mathcal F$ extends as its coordinate function. Rescaling therefore extends every bounded real [continuous function](../../../../../continuous-function.md); real and imaginary parts extend bounded complex [continuous functions](../../../../../continuous-function.md). The extension is unique because $X$ is dense and the target is [Hausdorff](../../../../../hausdorff-space.md). Its [supremum norm](../../../../../supremum-norm.md) is unchanged by density, so restriction is an [isometric isomorphism of normed spaces](../../../../../isometric-isomorphism-of-normed-spaces.md) of [Banach spaces](../../../../../banach-space-split.md)

$$
\boxed{C(\beta X)\cong C_b(X).}
$$

These are the [space of continuous functions on a compact space](../../../../../space-of-continuous-functions-on-a-compact-space.md) and the space of [bounded continuous functions](../../../../../bounded-continuous-functions.md), respectively.

More generally, embed a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) $K$ in its own evaluation cube $[0,1]^{C(K,[0,1])}$. This is an embedding by complete regularity, and its image is closed by compactness. For a [continuous map](../../../../../continuous-map.md) $u:X\to K$, extend all the bounded coordinates $f\circ u$ to $\beta X$. The resulting [continuous map](../../../../../continuous-map.md) into the cube takes its values in the closed copy of $K$: it does so on the dense subset $X$, and the inverse image of that closed copy is closed. Thus

$$
\boxed{u:X\to K\text{ extends uniquely to }\widetilde u:\beta X\to K.}
$$

Uniqueness again follows from density. This is the universal property of the [Stone-Čech compactification](../../../../../stone-cech-compactification.md). It implies uniqueness of the compactification up to a [homeomorphism](../../../../../homeomorphism.md) fixing $X$, by extending the identity in both directions. Every Hausdorff compactification of $X$ is the image of $\beta X$ under a continuous surjection fixing $X$, since that image is compact and contains the dense copy of $X$. A [continuous map](../../../../../continuous-map.md) $X\to Y$ between [completely regular Hausdorff spaces](../../../../../completely-regular-hausdorff-space.md) likewise extends uniquely to $\beta X\to\beta Y$ after composing with the embedding of $Y$; these extensions preserve identities and composition. If $X$ is already compact, its dense copy is closed, so $\beta X=X$.

For discrete $X$, every indicator $\mathbf1_D$, $D\subseteq X$, is continuous. Its extension to $\beta X$ takes only values $0,1$, since this closed condition holds on the dense subset $X$. Its one-set is precisely $\overline D$ and is [clopen](../../../../../clopen-set.md): it is closed, and every neighborhood of one of its points meets $D$ by density and continuity. This also gives the [discrete Stone-Čech compactifications are extremally disconnected](../../../../../discrete-stone-cech-compactifications-are-extremally-disconnected.md) property: for open $O$, density implies $\overline O=\overline{O\cap X}$, which is clopen.

For the requested separation, a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) is [normal](../../../../../normal-distribution.md), so [Urysohn's lemma](../../../../../urysohn-s-lemma.md) supplies $u:\beta X\to[0,1]$ with $u=0$ on $A$ and $u=1$ on $B$. Put $D=\{x\in X:u(x)<1/2\}$ and

$$
U=\overline D,\qquad V=\beta X\setminus U.
$$

The preceding indicator argument makes both sets clopen. At a point of $A$, the neighborhood $u<1/2$ has its dense $X$-part inside $D$, so the point lies in $U$. At a point of $B$, the neighborhood $u>1/2$ misses $D$, so the point lies outside $U$. We have proved the stronger [clopen separation in discrete Stone-Čech compactifications](../../../../../clopen-separation-in-discrete-stone-cech-compactifications.md) conclusion

$$
\boxed{\beta X=U\mathbin{\dot\cup}V,\qquad A\subseteq U,\quad B\subseteq V,\quad U,V\text{ clopen}.}
$$

Finally take **$\boxed{K=\beta\mathbb N}$**, the [Stone-Čech compactification of the natural numbers](../../../../../stone-cech-compactification-of-the-natural-numbers.md). It is a [compact Hausdorff space](../../../../../compact-hausdorff-space.md) and is [separable](../../../../../separable-topological-space.md), because its embedded copy of $\mathbb N$ is countable and dense. For every $D\subseteq\mathbb N$, the indicator extends to an element $h_D\in C(K)$. For distinct $D,D'$, evaluating at an integer in their symmetric difference gives $\|h_D-h_{D'}\|_\infty=1$. There are uncountably many such indicators. A separable [metric space](../../../../../metric-space.md) cannot contain an uncountable family at pairwise distance one: disjoint balls of radius $1/3$ would require distinct members of a countable dense set. Hence **$C(K)$ is not separable**, despite separability of $K$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
