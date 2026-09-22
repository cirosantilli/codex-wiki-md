<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $X=\operatorname{Spec}B$, $S=\operatorname{Spec}A$ with $A,B$ [integral domains](../../../../integral-domain.md), let $\alpha:A\to B$ be the [ring homomorphism](../../../../ring-homomorphism.md), and put $K=\operatorname{Frac}(B)$. We do not assume that $\alpha$ is injective. Write $A'=\alpha(A)\subseteq B\subseteq K$.

Let $D\subseteq K$ be any [valuation ring](../../../../valuation-ring.md) containing $A'$, with [fraction field](../../../../field-of-fractions.md) $K$. The canonical [morphism of schemes](../../../../morphism-of-schemes.md) $\operatorname{Spec}K\to\operatorname{Spec}B$ and the [ring homomorphism](../../../../ring-homomorphism.md) $A\to A'\hookrightarrow D$ form a valuative problem for $f$. Since $f$ is a [proper morphism](../../../../proper-morphism.md), there is an extension. On [coordinate rings](../../../../coordinate-ring.md) it is a [ring homomorphism](../../../../ring-homomorphism.md) $\beta:B\to D$ such that

$$
B\xrightarrow{\beta}D\hookrightarrow K
$$

is the original inclusion of $B$ into $K$. Therefore every element of $B$ lies in $D$. Since $D$ was arbitrary, the stated description of [integral closure as an intersection of valuation rings](../../../../integral-closure-as-an-intersection-of-valuation-rings.md) gives

$$
B\subseteq\bigcap_{\substack{D\subseteq K\text{ valuation ring}\\ A'\subseteq D}}D
=\overline{A'}^{\,K}.
$$

Thus every element of $B$ is an [integral element](../../../../integral-element.md) over $A'$, and hence over $A$: lift the coefficients of its [monic polynomial](../../../../monic-polynomial.md) along the surjection $A\to A'$. The [ring homomorphism](../../../../ring-homomorphism.md) $\alpha$ is therefore an [integral extension](../../../../integral-extension.md) in the sense of the question.

A [proper morphism](../../../../proper-morphism.md) is of [finite type](../../../../morphism-of-finite-type.md), so in this affine situation $B=A[b_1,\ldots,b_s]$. If $b_i$ satisfies a [monic polynomial](../../../../monic-polynomial.md) of degree $n_i$, repeatedly reducing its powers shows that the finitely many [monomials](../../../../monomial.md)

$$
b_1^{e_1}\cdots b_s^{e_s},\qquad 0\leq e_i<n_i,
$$

generate $B$ as an $A$-[module](../../../../module-mathematics.md). Equivalently, apply the allowed equivalence between finite and integral plus [finite type](../../../../morphism-of-finite-type.md). Hence

$$
\boxed{f\text{ proper between affine integral schemes}\Longrightarrow f\text{ finite}.}
$$

## ↑ Ancestors (12)

1. [E](../e.md)
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
