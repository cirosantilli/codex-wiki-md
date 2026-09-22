<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

All geometric [2-torsion](../../../../../2-torsion.md) is rational: its points are $O,(\alpha,0),(\beta,0),(\gamma,0)$. We will construct the required finite quotient directly, without assuming any theorem about finite generation or [two-descent on an elliptic curve](../../../../../two-descent-on-an-elliptic-curve.md).

Choose $Q\in E(\overline K)$ with $2Q=P$ and define the [halving cocycle with rational two-torsion](../../../../../halving-cocycle-with-rational-two-torsion.md)

$$
c_P(\sigma)=\sigma Q-Q\in E[2],\qquad \sigma\in G_K.
$$

Such a half exists because the nonconstant multiplication morphism $[2]$ on a smooth projective [elliptic curve](../../../../../elliptic-curve.md) is surjective over an [algebraic closure](../../../../../algebraic-closure.md). Since $E[2]$ is rational, $c_P(\sigma\tau)=c_P(\sigma)+c_P(\tau)$. A different half is $Q+T$ with rational $T\in E[2]$ and gives the same cocycle. Replacing $P$ by $P+2R$, with $R\in E(K)$, allows the half $Q+R$ and again changes nothing. Adding chosen halves shows additivity in $P$. If the cocycle is zero, the half is fixed by the [absolute Galois group](../../../../../absolute-galois-group.md) and lies in $E(K)$, so $P\in2E(K)$. This proves, rather than assumes, an injection

$$
E(K)/2E(K)\hookrightarrow\operatorname{Hom}_{\mathrm{cont}}(G_K,E[2]).
$$

The fixed field of $\ker c_P$ is exactly $K(Q)$. Its [Galois group](../../../../../galois-group.md) is the image of $c_P$, so its degree is at most four. This also follows from the permitted biquadratic description.

Let $S$ be the finite set of primes dividing $2(\alpha-\beta)(\alpha-\gamma)(\beta-\gamma)$. At a place $v\notin S$ the displayed integral cubic has unit [elliptic-curve discriminant](../../../../../elliptic-curve-discriminant.md), hence [good reduction of an elliptic curve](../../../../../good-reduction-of-an-elliptic-curve.md), and the residue characteristic is odd. Choose a half $\overline Q$ of the reduction of $P$ over the algebraic closure of the [residue field](../../../../../residue-field.md). Its coordinates belong to a finite residue extension; let $L_v/K_v$ be the corresponding finite [unramified extension](../../../../../unramified-extension.md). Smoothness and the [Hensel lemma](../../../../../hensel-s-lemma.md) lift $\overline Q$ to some $Q_0\in E(L_v)$. The difference $P-2Q_0$ reduces to zero and belongs to the [formal kernel of a minimal Weierstrass equation](../../../../../formal-kernel-of-a-minimal-weierstrass-equation.md). In its integral [formal group law](../../../../../formal-group-law.md) the doubling series is $2t+O(t^2)$, with unit linear coefficient. The [prime-to-residue-characteristic multiplication on a formal group](../../../../../prime-to-residue-characteristic-multiplication-on-a-formal-group.md) gives a unique $R$ in this kernel such that $2R=P-2Q_0$. Thus $Q_0+R$ is a half of $P$ defined over an unramified local extension. Every other half differs by rational [2-torsion](../../../../../2-torsion.md), so it too is unramified. We have proved the [unramified halving fields for a split cubic](../../../../../unramified-halving-fields-for-a-split-cubic.md) assertion at every $v\notin S$.

There are only finitely many [bounded-degree extensions with restricted ramification](../../../../../bounded-degree-extensions-with-restricted-ramification.md) of $K$ of degree at most four. This is the permitted number-field finiteness consequence of the [Hermite–Minkowski theorem](../../../../../hermite-minkowski-theorem.md): bounded local degrees bound the discriminant exponents at the finitely many allowed ramified primes, so absolute discriminants are bounded. Each possible halving field $L$ is Galois, and there are only finitely many homomorphisms $\operatorname{Gal}(L/K)\to E[2]$. The injection constructed above therefore has finite image. **Consequently $E(K)/2E(K)$ is finite.** No elliptic-curve finiteness or descent theorem was used in this argument.

For $K=\mathbb Q$, write $s=\#S$. Each coordinate of $c_P$ in a basis of $E[2]\cong(\mathbb Z/2\mathbb Z)^2$ is a quadratic [Galois character](../../../../../galois-character.md) unramified outside $S$. Its quadratic extension has a signed [square-free integer](../../../../../square-free-integer.md) representative $d=\pm\prod_{p\in S}p^{e_p}$, $e_p\in\{0,1\}$: an odd valuation outside $S$ would ramify there. There are at most $2^{s+1}$ choices, including the trivial character. Hence the pair of characters gives at most $2^{2s+2}$ cocycles. Each prime in $S$ is at most $2m$, because the three root differences have absolute values at most $2m$ and $2\leq2m$. Among the integers up to $2m$ there are at most $m$ primes: two, together with at most $m-1$ odd candidates. The [rational halving quotient bound from root size](../../../../../rational-halving-quotient-bound-from-root-size.md) is therefore

$$
\boxed{\#\bigl(E(\mathbb Q)/2E(\mathbb Q)\bigr)\leq2^{2s+2}\leq2^{2m+2}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
