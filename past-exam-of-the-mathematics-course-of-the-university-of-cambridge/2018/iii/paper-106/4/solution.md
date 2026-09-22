<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Mazur theorem](../../../../../mazur-theorem.md) states that the [weak closure](../../../../../weak-closure.md) and norm closure of a [convex set](../../../../../convex-set.md) $C$ in a [normed vector space](../../../../../normed-vector-space.md) coincide:

$$
\boxed{\overline C^{\,w}=\overline C^{\,\|\cdot\|}.}
$$

Norm closure is contained in [weak closure](../../../../../weak-closure.md) because the [weak topology](../../../../../weak-topology-split.md) is coarser. Conversely, if $x\notin\overline C^{\,\|\cdot\|}$, the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) provides a continuous real linear functional strictly separating $x$ from that closed [convex set](../../../../../convex-set.md). In a complex space this is the [real part](../../../../../real-part.md) of a continuous complex linear functional. A weak neighborhood of $x$ then misses $C$, so $x\notin\overline C^{\,w}$. This proves the equality. It also gives the usual [Mazur lemma](../../../../../mazur-s-lemma.md): if $x_n\rightharpoonup x$, then $x$ lies in the norm closure of the [convex hull](../../../../../convex-hull.md) of each tail, so one can choose tail [convex combinations](../../../../../convex-combination.md) $y_n$ with $\|y_n-x\|<1/n$.

Now let $K$ be a [weakly compact set](../../../../../weakly-compact-set.md) in a normed space $X$. Each $\varphi\in X^*$ is bounded on $K$ because it is weakly continuous. The family $\{Jx:x\in K\}$ in $\mathcal B(X^*,\mathbb F)$, where $J$ is the [canonical embedding into the bidual](../../../../../canonical-embedding-into-the-bidual.md), is therefore pointwise bounded. The space $X^*$ is Banach even if $X$ is not. Apply the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) and use $\|Jx\|=\|x\|$ to obtain

$$
\boxed{\sup_{x\in K}\|x\|<\infty.}
$$

This proves that a [weakly compact set is norm bounded](../../../../../weakly-compact-set-is-norm-bounded.md) without assuming completeness of the original space.

For the real-valued dual and integral formulas that follow, take $X$ to be real, as in the PDF. In a complex space the norming formula uses [real parts](../../../../../real-part.md), and the integral identities use complex-valued functionals instead.

If the [separable Banach space](../../../../../separable-banach-space.md) $X$ is nonzero, choose a norm-dense sequence $(u_n)$ in its unit sphere. By the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md), choose $\varphi_n\in X^*$ with $\|\varphi_n\|=1$ and $\varphi_n(u_n)=1$. For any unit vector $u$, arbitrarily close $u_n$ satisfy

$$
1-\|u-u_n\|\leq\varphi_n(u)\leq1.
$$

Scaling gives the [countable norming family](../../../../../countable-norming-family.md) identity

$$
\boxed{\|x\|=\sup_n\varphi_n(x)\quad(x\in X).}
$$

For $X=\{0\}$ use the constant sequence of zero functionals. If $f:\Omega\to X$ is norm-Borel measurable, every $\varphi_n\circ f$ is measurable, so its countable supremum $\|f(\cdot)\|$ is measurable. Equivalently, this also follows directly from continuity of the [norm](../../../../../norm.md).

For any $\varphi\in X^*$, continuity makes $\varphi\circ f$ measurable, and

$$
|\varphi(f(\omega))|\leq\|\varphi\|\,\|f(\omega)\|.
$$

Thus the assumed integrability of the norm implies scalar integrability, and

$$
T_f(\varphi)=\int_\Omega\varphi(f(\omega))\,d\mu(\omega),\qquad
|T_f(\varphi)|\leq\|\varphi\|\int_\Omega\|f\|\,d\mu
$$

defines a bounded linear functional on $X^*$. Use the granted weak-star continuity of $T_f$. By the [continuous dual of a weak-star topology](../../../../../continuous-dual-of-a-weak-star-topology.md), $T_f$ is evaluation at a vector of $X$. Indeed, continuity gives finitely many $x_1,\ldots,x_m$ and $\varepsilon>0$ such that $|T_f(\varphi)|<1$ whenever $|\varphi(x_j)|<\varepsilon$ for all $j$. Scaling shows that $T_f$ vanishes on the common kernel of these evaluations. It therefore factors through their finite-dimensional coordinate map, so $T_f(\varphi)=\sum_ja_j\varphi(x_j)=\varphi(\sum_ja_jx_j)$. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) makes this representing vector unique. Hence

$$
\boxed{v=\int_\Omega f\,d\mu\in X,\qquad \varphi(v)=\int_\Omega\varphi\circ f\,d\mu\quad(\varphi\in X^*),\qquad
\|v\|\leq\int_\Omega\|f\|\,d\mu.}
$$

In this separable setting the vector is the [Bochner integral](../../../../../bochner-integral.md).

Return to a [weakly compact set](../../../../../weakly-compact-set.md) $K\subseteq X$ and its inclusion $f:K\to X$. For each fixed $a\in X$, the identity $\|x-a\|=\sup_n\varphi_n(x-a)$ makes $x\mapsto\|x-a\|$ weakly Borel measurable. Norm balls are consequently weakly Borel measurable. Separability gives a countable base of such balls, so every norm-open set is weakly Borel measurable. This proves measurability of $f$, and establishes the equality of the [weak and norm Borel sigma-algebras in a separable Banach space](../../../../../weak-and-norm-borel-sigma-algebras-in-a-separable-banach-space.md).

Put $M=\sup_{x\in K}\|x\|<\infty$. For every finite signed [Borel measure](../../../../../borel-measure.md) $\mu$ on $K$,

$$
\boxed{\int_K\|f(x)\|\,d|\mu|(x)\leq M|\mu|(K)<\infty.}
$$

For positive measures this is the integral in the question. For signed measures, the correct integrability condition uses the [variation measure](../../../../../variation-measure.md); define the integral by taking the difference of the positive and negative integrals. The printed $\Omega$ in this clause should be $K$, the domain of the inclusion.

The [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) now defines the bounded linear map

$$
T:C(K)^*\to X,\qquad T(\mu)=\int_Kx\,d\mu(x),\qquad \|T(\mu)\|\leq M\|\mu\|_{\mathrm{TV}}.
$$

For each $\varphi\in X^*$ the restriction $\varphi|_K$ is in $C(K)$, and

$$
\varphi(T(\mu))=\mu(\varphi|_K).
$$

The right side is weak-star continuous in $\mu$. The defining property of the [weak topology](../../../../../weak-topology-split.md) therefore proves that $T$ is weak-star-to-weak continuous, for arbitrary nets. For a [Dirac measure](../../../../../dirac-measure.md), $\boxed{T(\delta_x)=x}$.

If $K\ne\varnothing$, let $\mathcal P(K)$ be its regular [probability measures](../../../../../probability-measure.md). This is a weak-star closed subset of $B_{C(K)^*}$: its conditions are $\mu(1)=1$ and $\mu(g)\geq0$ for every nonnegative $g\in C(K)$. It is compact by [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md). Thus $T(\mathcal P(K))$ is weakly compact and [convex](../../../../../convex-function.md), and contains $K$ because it contains all $T(\delta_x)$. It is weakly closed, hence norm closed, so it contains $C=\overline{\operatorname{conv}K}^{\,\|\cdot\|}$. By [Mazur theorem](../../../../../mazur-theorem.md), $C$ is weakly closed. Therefore it is a closed subset of the weakly compact set $T(\mathcal P(K))$, proving

$$
\boxed{\overline{\operatorname{conv}K}^{\,\|\cdot\|}\text{ is weakly compact}.}
$$

The empty case is immediate. In fact $T(\mathcal P(K))=C$: a [barycenter of a measure on a Banach space](../../../../../barycenter-of-a-measure-on-a-banach-space.md) outside $C$ would be strictly separated by a functional $\varphi$, contradicting $\varphi(T(\mu))=\int_K\varphi\,d\mu\leq\sup_K\varphi$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
