<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [divisor on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md) $D=\sum n_PP$, define its [line bundle associated to a divisor](../../../../../../line-bundle-associated-to-a-divisor.md) inside the [sheaf](../../../../../../sheaf-mathematics.md) of rational functions by

$$
\mathcal O_X(D)(U)=
\{f\in k(X)^*:v_P(f)+n_P\ge0\text{ for every }P\in U\}\cup\{0\}.
$$

Locally choose a rational equation $f_i$ for $D$, as in the construction of the quotient [sheaf](../../../../../../sheaf-mathematics.md) above. Then

$$
\mathcal O_X(D)|_{U_i}=f_i^{-1}\mathcal O_{U_i},
\qquad
\mathcal O_X(D)_P=t_P^{-n_P}\mathcal O_{X,P}.
$$

Consequently this is an [invertible sheaf](../../../../../../line-bundle.md). Multiplication gives an [isomorphism](../../../../../../isomorphism.md)

$$
\mathcal O_X(D)\otimes_{\mathcal O_X}\mathcal O_X(E)
\cong\mathcal O_X(D+E),
$$

as is checked on the displayed local generators. If $D=\operatorname{div}(f)$, multiplication by $f$ identifies $\mathcal O_X(D)$ with $\mathcal O_X$. Thus $D\mapsto[\mathcal O_X(D)]$ induces a [group homomorphism](../../../../../../group-homomorphism.md) from the [divisor class group](../../../../../../divisor-class-group.md) to the [Picard group](../../../../../../picard-group.md).

For surjectivity, let $\mathcal L$ be an [invertible sheaf](../../../../../../line-bundle.md). Trivialize its one-dimensional rational fibre over the [function field](../../../../../../function-field-of-an-algebraic-variety.md) $k(X)$; equivalently, choose a nonzero rational section and identify $\mathcal L$ with a subsheaf of the rational-function [sheaf](../../../../../../sheaf-mathematics.md). A finite trivializing cover gives

$$
\mathcal L|_{U_i}=a_i\mathcal O_{U_i},\qquad a_i\in k(X)^*.
$$

On overlaps $a_i/a_j$ is a regular unit. The integers $-v_P(a_i)$ therefore agree wherever two descriptions apply and define a finite [divisor on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md) $D$. Its local description gives $\mathcal L=\mathcal O_X(D)$. A different rational trivialization multiplies all $a_i$ by the same rational function, changing $D$ by a [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md), so the resulting [divisor class](../../../../../../divisor-class.md) is intrinsic.

For injectivity, an [isomorphism](../../../../../../isomorphism.md) $\mathcal O_X(D)\to\mathcal O_X(E)$ becomes multiplication by some $g\in k(X)^*$ on the rational fibre. At each closed point its effect on the local free generators gives

$$
g\,t_P^{-n_P(D)}\mathcal O_{X,P}
=t_P^{-n_P(E)}\mathcal O_{X,P},
\qquad
v_P(g)=n_P(D)-n_P(E).
$$

Hence $D-E=\operatorname{div}(g)$. Conversely this equality gives the required [isomorphism](../../../../../../isomorphism.md) by multiplication by $g$. We have proved the [group isomorphism](../../../../../../group-isomorphism.md)

$$
\boxed{\operatorname{Cl}(X)\xrightarrow{\;\sim\;}
\operatorname{Pic}(X),\qquad[D]\longmapsto[\mathcal O_X(D)].}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
