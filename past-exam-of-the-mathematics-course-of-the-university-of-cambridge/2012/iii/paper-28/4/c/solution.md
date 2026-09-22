<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We count extensions up to $K$-isomorphism. An extension of degree $n$ has a maximal [unramified extension](../../../../../../unramified-extension.md) $E/K$ inside it, with $[E:K]=f\mid n$, and $L/E$ is [totally ramified](../../../../../../totally-ramified-extension.md) of degree $e=n/f$. The unramified extension of each degree is unique, so there are only finitely many possibilities for $E$.

Fix $E$ and $e$. The coefficient space of monic degree-$e$ [Eisenstein polynomials](../../../../../../eisenstein-polynomial.md) is compact: its nonconstant nonleading coefficients lie in the compact [maximal ideal](../../../../../../maximal-ideal.md), and its constant coefficient lies in the compact set $\mathfrak m_E\setminus\mathfrak m_E^2$. Each such polynomial $F$ has a root $\alpha$ generating a degree-$e$ extension. For sufficiently close coefficients of a polynomial $G$, the numbers $G(\alpha)$ and $G'(\alpha)-F'(\alpha)$ are arbitrarily small, while $F'(\alpha)\ne0$ because the characteristic is zero. The [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md), applied in $E(\alpha)$, supplies a root $\beta$ of $G$ as close to $\alpha$ as desired. Choose the neighborhood so that the [Krasner's lemma](../../../../../../krasner-s-lemma.md) inequality holds. Then $E(\alpha)\subseteq E(\beta)$, and both degrees are $e$, so the extensions are equal. Compactness gives a finite cover by such neighborhoods, proving **finiteness of degree-$n$ extensions**. If extensions are realized as subfields of a fixed algebraic closure rather than counted up to isomorphism, each has only finitely many embeddings, so that count is finite too.

For odd $p$, write $K^\times=\pi^{\mathbb Z}\mathcal O_K^\times$. The square map is bijective on $1+\mathfrak m_K$ by [Hensel lemma](../../../../../../hensel-s-lemma.md), and the finite [residue field](../../../../../../residue-field.md) has cyclic multiplicative group of even order. Thus

$$
K^\times/K^{\times2}\cong(\mathbb Z/2\mathbb Z)^2.
$$

The [quadratic extensions from square classes](../../../../../../quadratic-extensions-from-square-classes.md) correspond to its three nontrivial classes. Representatives are $u,\pi,u\pi$, where $u$ is a unit with nonsquare residue. **There are $\boxed{3}$ [quadratic extensions](../../../../../../quadratic-extension.md): $K(\sqrt u)$ is unramified, while $K(\sqrt\pi)$ and $K(\sqrt{u\pi})$ are totally ramified.** For completeness, two nonsquare parameters give the same extension only if their ratio is a square: writing $\sqrt b=x+y\sqrt a$ and squaring forces $x=0$, hence $b/a=y^2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
