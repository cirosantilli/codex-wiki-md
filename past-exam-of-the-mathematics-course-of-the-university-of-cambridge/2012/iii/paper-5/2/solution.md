<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write a finite binary word as $s=(s_1,\ldots,s_n)$ and denote its prefix [cylinder set](../../../../../cylinder-set.md) by

$$
[s]=\{\omega:\omega_1=s_1,\ldots,\omega_n=s_n\}.
$$

More generally, a [cylinder set](../../../../../cylinder-set.md) fixes finitely many coordinates, or prescribes a subset of their finite coordinate product, leaving all other coordinates free. Each coordinate factor is discrete, so finite-coordinate inverse images are both open and closed. Thus cylinders are [clopen](../../../../../clopen-set.md). The basic open sets of the [product topology](../../../../../product-topology.md) restrict only finitely many coordinates, so cylinders form a base. Any finite-coordinate cylinder is a finite union of prefix cylinders of one sufficiently long common length; the prefix cylinders therefore also form a base.

The [Bernoulli space](../../../../../cantor-space.md) here is [Cantor space](../../../../../cantor-space.md), with compatible [metric](../../../../../metric.md)

$$
d(\omega,\omega')=\sum_{j\ge1}2^{-j}|\omega_j-\omega_j'|.
$$

It is a [compact metric space](../../../../../compact-metric-space.md): from any sequence, choose successively subsequences constant in the first, second and subsequent coordinates, and take the diagonal subsequence. Agreement on the first $n$ coordinates bounds the distance by $2^{-n}$, proving convergence. [Compactness](../../../../../compact-space.md) also follows from [Tychonoff theorem](../../../../../tychonoff-s-theorem.md).

Every cylinder [indicator function](../../../../../indicator-function.md) is continuous because the cylinder is [clopen](../../../../../clopen-set.md). Hence $S(\Omega)$ is a [vector subspace](../../../../../vector-subspace.md) of the [space of continuous functions on a compact space](../../../../../space-of-continuous-functions-on-a-compact-space.md). To prove density, fix $f\in C_{\mathbb R}(\Omega)$ and $\varepsilon>0$. By [uniform continuity](../../../../../uniform-continuity.md), choose $n$ so that $d(x,y)\le2^{-n}$ implies $|f(x)-f(y)|<\varepsilon$. Choose a point $\omega_s$ in each length-$n$ prefix cylinder and put

$$
f_n=\sum_{s\in\{0,1\}^n}f(\omega_s)1_{[s]}.
$$

Then $f_n\in S(\Omega)$ and $\|f-f_n\|_\infty<\varepsilon$. This proves [cylinder-function density in Cantor space](../../../../../cylinder-function-density-in-cantor-space.md):

$$
\boxed{\overline{S(\Omega)}^{\|\cdot\|_\infty}=C_{\mathbb R}(\Omega).}
$$

Positivity of $\phi$ implies monotonicity. The pointwise bounds $-\|f\|_\infty1\le f\le\|f\|_\infty1$ therefore give

$$
|\phi(f)|\le\|f\|_\infty\phi(1)=\|f\|_\infty.
$$

Evaluation on $1$ attains equality, so **$\phi$ is continuous and has norm one**. This is the [norm of a positive functional on C(K)](../../../../../norm-of-a-positive-functional-on-c-k.md).

The object extended to open sets is the set function $\ell(C)=\phi(1_C)$, rather than the functional $\phi$ itself. Positivity gives $\ell(C)\ge0$, and linearity gives finite additivity on disjoint cylinders. To construct its extension directly, use the [disjoint cylinder decomposition of open subsets of Cantor space](../../../../../disjoint-cylinder-decomposition-of-open-subsets-of-cantor-space.md). For an open $U$, take the shortest prefixes $s$ for which $[s]\subset U$. They are prefix-free, their cylinders are disjoint, and their union is $U$. Define

$$
\boxed{\ell(U)=\sum_{[s]\text{ in this decomposition}}\ell([s]).}
$$

For $U=\Omega$, use the empty prefix; for $U=\varnothing$, use the empty sum.

This value is independent of the chosen disjoint prefix-cylinder decomposition. Indeed, compare two such decompositions $(C_i)$ and $(D_j)$. For each fixed $C_i$, its intersections with the $D_j$ give a disjoint open cover of the compact cylinder $C_i$. [Compactness](../../../../../compact-space.md) reduces this to finitely many nonempty intersections. Each intersection is a prefix cylinder or is empty, so finite additivity gives $\ell(C_i)=\sum_j\ell(C_i\cap D_j)$. Sum over $i$ and rearrange the nonnegative double sum. Doing the same with each $D_j$ proves equality of the two totals.

For disjoint open sets $U_k$, combine their disjoint cylinder decompositions to obtain one for $\bigcup_kU_k$. Rearrangement of nonnegative sums proves [countable additivity](../../../../../countable-additivity.md) on this family of open sets. The extension is unique because any countably additive extension must have the prescribed sum on every disjoint cylinder decomposition. Open sets are not themselves a [sigma-algebra](../../../../../sigma-algebra.md); [countable additivity](../../../../../countable-additivity.md) here concerns disjoint open families and their open union.

For the [Borel probability measure](../../../../../borel-probability-measure.md), let $\mathcal A$ be the algebra of finite unions of prefix cylinders. It is also the algebra of [clopen sets](../../../../../clopen-set.md), because every clopen set is compact and has a finite cylinder cover. Define $\ell(A)=\phi(1_A)$ on $\mathcal A$. If $A=\bigsqcup_{k\ge1}A_k$ with all sets in $\mathcal A$, [compactness](../../../../../compact-space.md) of $A$ gives a finite subcover by the $A_k$. Disjointness makes all remaining members empty. Thus finite additivity already establishes the [premeasure](../../../../../premeasure.md) condition.

The [Caratheodory extension theorem](../../../../../caratheodory-s-extension-theorem.md) gives a unique [measure](../../../../../measure.md) $P$ on $\sigma(\mathcal A)$. This is the [Borel sigma-algebra](../../../../../borel-sigma-algebra.md), since the cylinders are a countable base; $P(\Omega)=1$. Its values on open sets agree with the extension above. For cylinder [simple functions](../../../../../simple-function.md),

$$
\phi(f_n)=\int_\Omega f_n\,dP.
$$

Both sides are continuous in the [supremum norm](../../../../../supremum-norm.md), so [cylinder-function density in Cantor space](../../../../../cylinder-function-density-in-cantor-space.md) gives

$$
\boxed{\phi(f)=\int_\Omega f\,dP\qquad(f\in C_{\mathbb R}(\Omega)).}
$$

Any other [Borel probability measure](../../../../../borel-probability-measure.md) with this property agrees on every cylinder [indicator function](../../../../../indicator-function.md), hence on $\mathcal A$, and uniqueness in the [Caratheodory extension theorem](../../../../../caratheodory-s-extension-theorem.md) makes it equal to $P$. This proves the [Cantor-space representation of positive functionals](../../../../../cantor-space-representation-of-positive-functionals.md) without assuming the general representation theorem.

Now let $h:\Omega\to X$ be the supplied continuous surjection. The pullback

$$
J:C_{\mathbb R}(X)\longrightarrow C_{\mathbb R}(\Omega),\qquad Jf=f\circ h
$$

is a unital [isometric embedding](../../../../../isometric-embedding.md): surjectivity gives $\|f\circ h\|_\infty=\|f\|_\infty$. On the [vector subspace](../../../../../vector-subspace.md) $J(C_{\mathbb R}(X))$, define $L(Jf)=\phi(f)$. This is well-defined, has norm one and satisfies $L(1)=1$.

The real [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) extends $L$ to $\widetilde L$ on all of $C_{\mathbb R}(\Omega)$ with the same norm. Norm preservation alone does not automatically mean positivity, so verify it. If $0\le g\le1$, then $\|1-g\|_\infty\le1$ and

$$
\widetilde L(g)=1-\widetilde L(1-g)\ge1-|\widetilde L(1-g)|\ge0.
$$

Scaling proves positivity for every nonnegative $g$. This is the [unital contraction positivity criterion](../../../../../unital-contraction-positivity-criterion.md), giving a [positive extension from a unital subspace of C(K)](../../../../../positive-extension-from-a-unital-subspace-of-c-k.md).

Represent $\widetilde L$ by the already constructed [Borel probability measure](../../../../../borel-probability-measure.md) $P$ on $\Omega$ and take the [pushforward measure](../../../../../pushforward-measure.md) $Q=h_*P$. Continuity of $h$ makes its Borel inverse images measurable, and $Q(X)=1$. The pushforward integral identity gives

$$
\boxed{\phi(f)=\widetilde L(f\circ h)
=\int_\Omega f\circ h\,dP=\int_Xf\,dQ.}
$$

This is [compact-metric representation by Cantor-space pullback](../../../../../compact-metric-representation-by-cantor-space-pullback.md). The hypothesis $\phi(1)=1$ already excludes an empty $X$. The [measure](../../../../../measure.md) is on the Borel sets; no uniqueness claim on an unspecified larger collection of subsets is needed.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
