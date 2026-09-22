<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $S=R^G$, the [ring of invariants](../../../../../../ring-of-invariants.md). It is an [integral domain](../../../../../../integral-domain.md) because it is a [subring](../../../../../../subring.md) of the domain $R$. Embed $\operatorname{Frac}S$ in $\operatorname{Frac}R$ in the evident way.

Suppose $q\in\operatorname{Frac}S$ is an [integral element](../../../../../../integral-element.md) over $S$. Its monic equation has coefficients in $S\subseteq R$, so $q$ is integral over $R$. Since $R$ is a [normal domain](../../../../../../integrally-closed-domain.md), $q\in R$.

Write $q=a/b$ with $a,b\in S$ and $b\ne0$. Each [ring automorphism](../../../../../../ring-automorphism.md) in $G$ extends to the [fraction field](../../../../../../field-of-fractions.md) by acting on numerator and denominator, and fixes this fraction. Hence $q\in R^G=S$. We have proved that $S$ is integrally closed in its own [fraction field](../../../../../../field-of-fractions.md):

$$
\boxed{R^G\text{ is a normal domain}}.
$$

This [normality of a ring of invariants](../../../../../../normality-of-a-ring-of-invariants.md) argument actually works for any group; finiteness is not needed for this conclusion. For finite $G$, there is additionally an [integral extension](../../../../../../integral-extension.md) $R^G\subseteq R$, since for each $r\in R$ the [orbit polynomial under a finite automorphism group](../../../../../../orbit-polynomial-under-a-finite-automorphism-group.md)

$$
\prod_{g\in G}(T-g(r))
$$

is monic, has coefficients fixed by $G$ and vanishes at $r$. Neither argument divides by $|G|$, so it is valid when the characteristic divides the group order. Here normality means integral closedness of a domain.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
