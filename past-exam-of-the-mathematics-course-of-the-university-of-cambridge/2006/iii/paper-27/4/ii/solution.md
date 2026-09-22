<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Krasner's lemma](../../../../../../krasner-s-lemma.md) states: let $K$ be [complete](../../../../../../completeness.md) for a [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md), let $\alpha$ be a [separable algebraic element](../../../../../../separable-algebraic-element.md) over $K$, and let $\beta$ be algebraic over $K$, all in a fixed [algebraic closure](../../../../../../algebraic-closure.md) with the extended [field absolute value](../../../../../../absolute-value-algebra.md). If

$$
|\beta-\alpha|<|\alpha'-\alpha|\quad\text{for every }K\text{-conjugate }\alpha'\ne\alpha,
$$

then $K(\alpha)\subseteq K(\beta)$. If $\alpha\in K$, the conclusion is automatic and there is no conjugate-distance condition to check.

To prove it, put $F=K(\beta)$ and take a finite splitting field $N/F$ for the minimal polynomial of $\alpha$ over $F$. That is a [separable polynomial](../../../../../../separable-polynomial.md), so $N/F$ is Galois. The finite extension $F$ is [complete](../../../../../../completeness.md), and uniqueness of extensions of an [field absolute value](../../../../../../absolute-value-algebra.md) from a [complete](../../../../../../completeness.md) non-Archimedean field makes every $\sigma\in\operatorname{Gal}(N/F)$ an isometry. It fixes $\beta$, so

$$
|\sigma(\alpha)-\alpha|\le\max\{|\sigma(\alpha)-\beta|,|\beta-\alpha|\}=|\beta-\alpha|.
$$

If $\sigma(\alpha)\ne\alpha$, it is another $K$-conjugate and this inequality contradicts the strict hypothesis. Every such automorphism therefore fixes $\alpha$. The [Fundamental theorem of Galois theory](../../../../../../fundamental-theorem-of-galois-theory.md) gives $\alpha\in F$, proving

$$
\boxed{K(\alpha)\subseteq K(\beta).}
$$

Only $\alpha$ needs to be a [separable algebraic element](../../../../../../separable-algebraic-element.md): the proof works even when $\beta$ is inseparable, because the splitting field is taken over $K(\beta)$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
