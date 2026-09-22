<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [line bundle](../../../../../../line-bundle.md) $\mathcal L$ is a [globally generated line bundle](../../../../../../globally-generated-line-bundle.md) when the evaluation map

$$
H^0(X,\mathcal L)\otimes_k\mathcal O_X\longrightarrow\mathcal L
$$

is surjective. Equivalently, its [global sections](../../../../../../global-section.md) span each fibre of the [line bundle](../../../../../../line-bundle.md); locally at every point, some section is a generator.

Choose a finite generating family $s_0,\ldots,s_n$. On the open set where $s_i$ generates $\mathcal L$, the ratios $s_j/s_i$ are regular functions, giving a [morphism of schemes](../../../../../../morphism-of-schemes.md) into the standard chart $D_+(x_i)$ of [projective space](../../../../../../projective-space-split.md). The ratios obey the usual transition rules on overlaps, so these chart maps glue to

$$
\boxed{\varphi:X\longrightarrow\mathbb P^n_k,\qquad x\longmapsto[s_0(x):\cdots:s_n(x)].}
$$

The tuple is computed using any local trivialization of $\mathcal L$; changing that trivialization multiplies all entries by the same invertible function. The construction has $\varphi^*\mathcal O(1)\simeq\mathcal L$ and pulls back the coordinate sections to the chosen $s_i$.

There is a finiteness qualification for an arbitrary $X$: global generation alone need not provide such a finite family. It does if $X$ is [quasi-compact](../../../../../../compact-space.md), since the open sets on which individual sections generate have a finite subcover. Without that hypothesis, take $X=\coprod_{m\geq1}\mathbb P^m_k$ and let $\mathcal L$ restrict to $\mathcal O(1)$ on each component. This [line bundle](../../../../../../line-bundle.md) is globally generated, but any $N$ global sections have a common zero on a component $\mathbb P^m$ with $m\geq N$. Thus this is a [globally generated line bundle without finite generators](../../../../../../globally-generated-line-bundle-without-finite-generators.md). This is [finite global generation on a quasi-compact scheme](../../../../../../finite-global-generation-on-a-quasi-compact-scheme.md). The finite-family construction is automatic in the projective case asked next.

For projective nonsingular $X$, put $V=\langle s_0,\ldots,s_n\rangle$. **The [length-two criterion for a very ample linear system](../../../../../../length-two-criterion-for-a-very-ample-linear-system.md) says that $\varphi$ is a [closed immersion](../../../../../../closed-immersion.md) precisely when, after extending to an algebraic closure, $V$ separates distinct points and tangent directions.** Equivalently, the evaluation

$$
V\longrightarrow H^0(E,\mathcal L|_E)
$$

is surjective for every length-two geometric [closed subscheme](../../../../../../closed-subscheme.md) $E\subseteq X$. Two distinct points give point separation; a nonreduced length-two subscheme supported at one point gives separation of a direction in the [Zariski tangent space](../../../../../../zariski-tangent-space.md). For the complete space $V=H^0(X,\mathcal L)$, this says exactly that $\mathcal L$ is a [very ample line bundle](../../../../../../very-ample-line-bundle.md). For a chosen smaller $V$, it is the chosen [linear system of divisors](../../../../../../linear-system-of-divisors.md) which must be a [very ample linear system](../../../../../../very-ample-linear-system.md); mere global generation is insufficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
