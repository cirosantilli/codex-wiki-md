<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $f_x$ for the [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) specified at $x$. Choose a cofinal sequence $V_i$ from the indexing family $I$, and write the target part of the supplied [subordinate flag for a family of linear isometries](../../../../../../subordinate-flag-for-a-family-of-linear-isometries.md) as $W_i$. After a cofinal enlargement it has

$$
V_i\subset V_{i+1},\qquad W_i\subset W_{i+1},\qquad f_x(V_i)\subset W_i\quad(x\in X).
$$

Both flags exhaust their [universe for spectra](../../../../../../universe-for-spectra.md). Compactness of the parameter space ensures that a finite target stage can contain all images of each fixed source stage.

Let $\xi_i$ be the [vector bundle](../../../../../../vector-bundle.md) on $X$ with fiber

$$
(\xi_i)_x=W_i\ominus f_x(V_i).
$$

Here $\ominus$ is the [orthogonal complement](../../../../../../orthogonal-complement.md) in the indicated ambient subspace. Its rank is $\dim W_i-\dim V_i$. Let $\operatorname{Th}(\xi_i)$ be its [Thom space](../../../../../../thom-space.md), the disk bundle modulo its sphere bundle, so that every fiber is compactified and all its points at infinity become the single basepoint. For the zero bundle this convention gives $\operatorname{Th}(0_X)=X_+$. Define a target [indexed prespectrum](../../../../../../indexed-prespectrum.md) on the flag by

$$
P(W_i)=\operatorname{Th}(\xi_i)\wedge E(V_i).
$$

The [smash product](../../../../../../smash-product.md) here is of [based spaces](../../../../../../based-space.md), not yet the derived [smash product of spectra](../../../../../../smash-product-of-spectra.md).

To specify all structure maps, for $i\le j$ use the continuous fiberwise orthogonal isomorphism

$$
(W_j\ominus W_i)\oplus(\xi_i)_x\cong(\xi_j)_x\oplus f_x(V_j\ominus V_i).
$$

Both sides identify with the complement of $f_x(V_i)$ in $W_j$. In particular this is the isometry obtained by orthogonally projecting onto $f_x(V_j\ominus V_i)$ and its complement; it is not an assertion that the displayed summands coincide separately. Pass to fiberwise [one-point compactifications](../../../../../../alexandroff-extension.md), identify the last summand with $V_j\ominus V_i$ using $f_x^{-1}$, and apply the source structure map. This defines

$$
S^{W_j\ominus W_i}\wedge P(W_i)\longrightarrow P(W_j).
$$

More explicitly, decompose $z+w\in W_j\ominus f_x(V_i)$, where $z\in W_j\ominus W_i$ and $w\in(\xi_i)_x$, as $w'+f_x(v)$ with $w'\in(\xi_j)_x$ and $v\in V_j\ominus V_i$. Send its pair with $e\in E(V_i)$ to the pair $(w',\sigma_{V_i,V_j}(v,e))$ over $x$. The notation for finite vectors extends to the compactifications, sending infinities and basepoints to the basepoint. Orthogonal decomposition and associativity of the source structure maps prove the prespectrum identities.

Extend the [indexed prespectrum](../../../../../../indexed-prespectrum.md) from the cofinal flag to the target indexing family and apply [spectrification](../../../../../../spectrification.md) $L$. The point-set definition is

$$
\boxed{X\ltimes_f E=LP.}
$$

On a [map of topological spectra](../../../../../../map-of-topological-spectra.md) $u:E\to E'$ it is induced at stage $i$ by $1_{\operatorname{Th}(\xi_i)}\wedge u(V_i)$. Thus the prescribed isometry family, indexing family and flag have all been used. A common cofinal refinement identifies the resulting objects in the [stable homotopy category](../../../../../../stable-homotopy-category.md); the point-set model retains the chosen flag. If $f$ is a constant standard inclusion, the complement bundles are trivial and this recovers the usual reindexed $X_+\wedge E$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
