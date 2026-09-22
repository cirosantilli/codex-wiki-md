<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the simple-root form of the [Hensel lemma](../../../../../../hensel-s-lemma.md): for $F\in\mathcal O_K[T]$ and $\bar a\in k_K$ satisfying $\overline F(\bar a)=0$ and $\overline{F'}(\bar a)\ne0$, there is a unique $a\in\mathcal O_K$ with $\bar a$ as its reduction and $F(a)=0$.

Let $d=[\ell:k_K]$. The [residue field](../../../../../../residue-field.md) $k_K$ is finite, so $\ell/k_K$ is separable, and the [primitive element theorem](../../../../../../primitive-element-theorem.md) gives $\ell=k_K(\bar\alpha)$. Let $\bar F$ be the monic irreducible polynomial of $\bar\alpha$, of degree $d$, and choose a monic coefficient lift $F\in\mathcal O_K[T]$. Irreducible reduction implies that $F$ is irreducible over $K$: any monic factorization over $K$ has integral coefficients, since all its roots are integral over the [valuation ring](../../../../../../valuation-ring.md), and would reduce to a factorization of $\bar F$.

Adjoin a root $\alpha$ and put $L=K(\alpha)$. Then $[L:K]=d$ and $\alpha\in\mathcal O_L$. Its reduction satisfies $\bar F$, so $k_L$ contains a copy of $\ell$ over $k_K$. For finite extensions of non-Archimedean [local fields](../../../../../../local-field.md), the fundamental degree relation is

$$
[L:K]=e(L/K)[k_L:k_K].
$$

The residue degree is at least $d$, while the left side equals $d$, hence

$$
\boxed{e(L/K)=1,\qquad k_L\cong\ell,\qquad [L:K]=[\ell:k_K].}
$$

This constructs the required [unramified extension](../../../../../../unramified-extension.md).

For uniqueness, let $L'/K$ be another unramified extension with a chosen identification $k_{L'}\cong\ell$. The element corresponding to $\bar\alpha$ is a simple residue root of $F$, because finite fields are perfect. The [Hensel lemma](../../../../../../hensel-s-lemma.md) in $L'$ gives a root $\alpha'\in\mathcal O_{L'}$ with this reduction. Since $F$ is irreducible of degree $d$, $[K(\alpha'):K]=d=[L':K]$, so $L'=K(\alpha')$. Sending $\alpha$ to $\alpha'$ yields a $K$-isomorphism $L\to L'$, compatible with the prescribed residue identification. Thus

$$
\boxed{\text{the unramified lift of }\ell/k_K\text{ is unique up to }K\text{-isomorphism}.}
$$

This proves the [existence and uniqueness of unramified local extensions](../../../../../../existence-and-uniqueness-of-unramified-local-extensions.md) using the stated version of Hensel's lemma, without assuming the classification in advance.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
