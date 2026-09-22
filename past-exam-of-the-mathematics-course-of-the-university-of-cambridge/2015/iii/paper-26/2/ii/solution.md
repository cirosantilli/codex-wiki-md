<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**A number-field completion is finite.** Let $F$ be the given [number field](../../../../../../number-field.md) and $L=F_{\mathfrak p}$ its completion. Normalize its [absolute value on a field](../../../../../../absolute-value-algebra.md) so that the restriction to $\mathbb Q$ is $|\cdot|_p$: if $v_{\mathfrak p}(p)=e$, use $|x|=p^{-v_{\mathfrak p}(x)/e}$. Changing the original absolute value by this positive power does not change its completion. The closure of $\mathbb Q$ in $L$ is an isometric copy of $\mathbb Q_p$.

Take a $\mathbb Q$-basis of $F$ and let $V$ be its $\mathbb Q_p$-span in $L$. Choose a maximal linearly independent subset of that finite spanning set. The [compact-sphere proof of finite-dimensional non-Archimedean norm equivalence](../../../../../../compact-sphere-proof-of-finite-dimensional-non-archimedean-norm-equivalence.md) applies to this basis too, so $V$ is complete and therefore closed in $L$. Since $F\subset V$ is dense in $L$, it follows that $V=L$. Hence

$$
\boxed{[F_{\mathfrak p}:\mathbb Q_p]\leq[F:\mathbb Q]<\infty.}
$$

**Every finite extension is obtained this way.** Let $E/\mathbb Q_p$ be finite. Use its extending [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md), whose completeness and uniqueness were proved above. In characteristic zero the [primitive element theorem](../../../../../../primitive-element-theorem.md) gives $E=\mathbb Q_p(\alpha)$; scaling $\alpha$ by a power of $p$, we may arrange that it is integral. Its monic minimal polynomial $f$ belongs to $\mathbb Z_p[T]$. If the degree is one, $E=\mathbb Q_p$ is already the completion of $\mathbb Q$.

Otherwise choose

$$
0<\delta<\min_{\alpha'\ne\alpha}|\alpha-\alpha'|,
$$

where $\alpha'$ runs over the conjugates in an algebraic closure. Approximate the coefficients of $f$ by integers, obtaining a monic $g\in\mathbb Z[T]$ of the same degree. Since $f'(\alpha)\ne0$, sufficiently accurate approximation gives $|g(\alpha)|<|g'(\alpha)|^2$ and makes $|g(\alpha)/g'(\alpha)|<\delta$. The [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md) in $E$ produces a root $\beta\in E$ of $g$ with $|\beta-\alpha|<\delta$.

For completeness, the required [Krasner's lemma](../../../../../../krasner-s-lemma.md) follows from the [unique extension of an absolute value to a finite extension](../../../../../../unique-extension-of-an-absolute-value-to-a-finite-extension.md). In a finite [Galois extension](../../../../../../finite-galois-extension.md) containing $\alpha,\beta$, every automorphism $\sigma$ fixing $\beta$ is an isometry, and

$$
|\sigma\alpha-\alpha|
\leq\max(|\sigma\alpha-\beta|,|\beta-\alpha|)
=|\alpha-\beta|.
$$

If $\sigma\alpha\ne\alpha$, this contradicts the choice of $\delta$. Thus every automorphism fixing $\beta$ fixes $\alpha$, and [Galois correspondence](../../../../../../galois-correspondence.md) gives $\mathbb Q_p(\alpha)\subseteq\mathbb Q_p(\beta)$. Since $\beta\in E$, equality follows. In particular $g$ is irreducible over $\mathbb Q_p$, and therefore over $\mathbb Q$.

Put $F=\mathbb Q(\beta)\subset E$. It is a [number field](../../../../../../number-field.md), and the closure of $F$ in $E$ contains $\mathbb Q_p(\beta)=E$, so $F$ is dense. Let

$$
\mathfrak p=\{b\in\mathcal O_F:|b|<1\}.
$$

Every element of the [ring of integers of a number field](../../../../../../ring-of-integers.md) has absolute value at most one: otherwise its highest-degree term would strictly dominate all other terms of a monic integer equation. Thus reduction into the [residue field](../../../../../../residue-field.md) of $E$ makes $\mathfrak p$ a [prime ideal](../../../../../../prime-ideal.md), and $\mathfrak p\cap\mathbb Z=p\mathbb Z$. The restriction of the [valuation](../../../../../../valuation.md) to $F$ is the [valuation](../../../../../../valuation.md) of this prime, up to normalization. Indeed, the localized [discrete valuation ring](../../../../../../discrete-valuation-ring.md) $(\mathcal O_F)_{\mathfrak p}$ maps into $\mathcal O_E$, its units have absolute value one, and its [uniformizer](../../../../../../uniformizer.md) has absolute value less than one. Density and completeness give

$$
\boxed{F_{\mathfrak p}\cong E.}
$$

This proves the [local realization as a completion of a number field](../../../../../../local-realization-as-a-completion-of-a-number-field.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
