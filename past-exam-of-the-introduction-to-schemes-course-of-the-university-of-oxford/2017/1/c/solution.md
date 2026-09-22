<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes.** First, the hypothesis implies that $f(T)$ is injective for every [scheme](../../../../scheme.md) $T$, even when $T$ is not an [affine scheme](../../../../affine-scheme.md). Indeed, suppose $a,b:T\to X$ satisfy $f\circ a=f\circ b$. Choose an [affine open cover](../../../../affine-open-cover.md) $T=\bigcup_\lambda V_\lambda$. On each $V_\lambda$, injectivity of $f(V_\lambda)$ gives $a|_{V_\lambda}=b|_{V_\lambda}$. By [gluing morphisms of schemes](../../../../gluing-morphisms-of-schemes.md), $a=b$.

Now choose an [affine open cover](../../../../affine-open-cover.md) $Y=\bigcup_i U_i$, and denote its inclusion maps by $j_i:U_i\hookrightarrow Y$. Surjectivity of $f(U_i)$ gives [morphisms of schemes](../../../../morphism-of-schemes.md) $g_i:U_i\to X$ with $f\circ g_i=j_i$. On $U_i\cap U_j$, the two restrictions have the same composite with $f$. By the injectivity just established for arbitrary test [schemes](../../../../scheme.md),

$$
g_i|_{U_i\cap U_j}=g_j|_{U_i\cap U_j}.
$$

In particular, the overlaps need not be [affine schemes](../../../../affine-scheme.md). [Gluing morphisms of schemes](../../../../gluing-morphisms-of-schemes.md) supplies $g:Y\to X$ with $g|_{U_i}=g_i$, and $f\circ g=1_Y$ because this holds on every $U_i$.

Finally,

$$
f\circ(g\circ f)=f=f\circ1_X.
$$

Injectivity of $f(X)$, already proved without an affineness assumption, gives $g\circ f=1_X$. Therefore

$$
\boxed{f\text{ is an isomorphism of schemes}.}
$$

This proves the relevant instance of [affine test schemes determine scheme morphisms](../../../../affine-test-schemes-determine-scheme-morphisms.md): the restricted [functor of points](../../../../functor-represented-by-a-scheme.md) still retains the information needed to construct the inverse.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
