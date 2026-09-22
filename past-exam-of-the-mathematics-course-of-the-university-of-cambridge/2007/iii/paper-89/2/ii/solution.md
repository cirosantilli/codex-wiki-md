<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $K\subseteq L^p$. Every $a\in A$ has a unique $p$th root $r(a)$ in $L$: existence is the [field](../../../../../../field.md) inclusion and uniqueness follows from injectivity of the [Frobenius endomorphism](../../../../../../frobenius-endomorphism.md) in a [field](../../../../../../field.md). Since $r(a)^p=a$, this root satisfies the monic polynomial $T^p-a$ over $B$. Because $B$ is an [integrally closed domain](../../../../../../integrally-closed-domain.md), this gives $r(a)\in B$. The identities

$$
(r(a)+r(a'))^p=a+a',\qquad (r(a)r(a'))^p=aa'
$$

and uniqueness show that

$$
\eta_V:A\longrightarrow B,\qquad a\longmapsto r(a)
$$

is a [ring homomorphism](../../../../../../ring-homomorphism.md).

On $D(a)$ the rule sends a fraction to the fraction of its unique roots. Since $r(a)^p=a$, inverting $a$ is equivalent to inverting $r(a)$, so the rule localizes. Also, for a prime $\mathfrak q\subset B$, $r(a)\in\mathfrak q$ exactly when $a\in\mathfrak q$; hence the induced point map agrees with that of $f$. The localized rules consequently glue to a morphism $h:X\to Y$. Its pullback followed by the [Frobenius endomorphism](../../../../../../frobenius-endomorphism.md) sends $a$ to $r(a)^p=a$, which proves

$$
\boxed{f=h\circ F_X.}
$$

If another morphism satisfies this equation, it has the same point map because the [Absolute Frobenius morphism](../../../../../../absolute-frobenius-morphism.md) fixes points, and its pullback of $a$ must be a $p$th root of $a$ in the [normal domain](../../../../../../integrally-closed-domain.md) $B$. That root is unique. Thus $h$ is unique.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 89](../../../paper-89-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
