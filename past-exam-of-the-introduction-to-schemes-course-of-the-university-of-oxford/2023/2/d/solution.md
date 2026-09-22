<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $D$ be a [valuation ring](../../../../valuation-ring.md), $K$ its [fraction field](../../../../field-of-fractions.md), and let $u:\operatorname{Spec}K\to X$, $v:\operatorname{Spec}D\to S$ be a compatible pair. Since $D$ is a [local ring](../../../../local-ring.md), every [open subset](../../../../open-set.md) of $\operatorname{Spec}D$ containing its unique [closed point](../../../../closed-point.md) is the whole space: a [principal open subset](../../../../principal-open-subscheme.md) containing the [maximal ideal](../../../../maximal-ideal.md) is defined by a [unit](../../../../unit-in-a-ring.md). Choose an [affine open subscheme](../../../../affine-open-subscheme.md) $V=\operatorname{Spec}A\subseteq S$ containing the image under $v$ of that [closed point](../../../../closed-point.md). The entire $v$ factors through $V$.

Because $f$ is a [finite morphism](../../../../finite-morphism.md), $f^{-1}(V)=\operatorname{Spec}B$ with $B$ a finite $A$-[module](../../../../module-mathematics.md). The valuative problem is the compatible [ring homomorphisms](../../../../ring-homomorphism.md)

$$
A\longrightarrow D\subseteq K,\qquad \psi:B\longrightarrow K.
$$

Every $b\in B$ is an [integral element](../../../../integral-element.md) over $A$. Mapping its [monic polynomial](../../../../monic-polynomial.md) equation to $K$ proves that $\psi(b)$ is an [integral element](../../../../integral-element.md) over $D$. Part (c) gives $\psi(b)\in D$. Thus $\psi$ factors uniquely as a [ring homomorphism](../../../../ring-homomorphism.md) $B\to D\hookrightarrow K$, producing the unique extension $\operatorname{Spec}D\to X$.

For completeness, a [finite morphism](../../../../finite-morphism.md) is a [quasi-compact morphism](../../../../quasi-compact-morphism.md) and of [finite type](../../../../morphism-of-finite-type.md): over $V$ its inverse image is an [affine scheme](../../../../affine-scheme.md), and finite $A$-[module](../../../../module-mathematics.md) generators also generate it as an $A$-[algebra](../../../../algebra-split.md). It is also a [separated morphism](../../../../separated-morphism.md). Affine-locally its [diagonal morphism](../../../../diagonal-morphism.md) corresponds to the surjective multiplication [ring homomorphism](../../../../ring-homomorphism.md)

$$
B\otimes_AB\longrightarrow B,\qquad b\otimes c\longmapsto bc,
$$

and hence is a [closed immersion](../../../../closed-immersion.md). In particular it is a [quasi-separated morphism](../../../../quasi-separated-morphism.md). The [valuative criterion for properness](../../../../valuative-criterion-for-properness.md) now applies, giving

$$
\boxed{f\text{ finite}\Longrightarrow f\text{ proper}.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
