<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $X\xrightarrow fY\xrightarrow gS$ be [morphisms of schemes](../../../../../morphism-of-schemes.md). Start with $u:\operatorname{Spec}K\to X$ and $v:\operatorname{Spec}D\to S$ satisfying $gfu=v|_{\operatorname{Spec}K}$.

For existence, first apply the extension condition for $g$ to $fu$ and $v$, obtaining $w:\operatorname{Spec}D\to Y$. Then apply the extension condition for $f$ to $u,w$, obtaining $\ell:\operatorname{Spec}D\to X$. This $\ell$ solves the problem for $gf$. If both $f,g$ are [universally closed morphisms](../../../../../universally-closed-morphism.md), both are [quasi-compact morphisms](../../../../../quasi-compact-morphism.md); their composite is a [quasi-compact morphism](../../../../../quasi-compact-morphism.md) by the allowed stability fact. Part (a)(i) therefore proves that $gf$ is a [universally closed morphism](../../../../../universally-closed-morphism.md).

For uniqueness, suppose $\ell_1,\ell_2$ are extensions for $gf$. Uniqueness for $g$ gives $f\ell_1=f\ell_2=w$, and uniqueness for $f$, now over this same $w$, gives $\ell_1=\ell_2$. If $f,g$ are [separated morphisms](../../../../../separated-morphism.md), their composite is a [quasi-separated morphism](../../../../../quasi-separated-morphism.md) by the allowed stability fact. Part (a)(ii) proves that $gf$ is a [separated morphism](../../../../../separated-morphism.md).

Finally, if $f,g$ are [proper morphisms](../../../../../proper-morphism.md), these arguments give both existence and uniqueness. Stability under composition of [quasi-compact morphisms](../../../../../quasi-compact-morphism.md), [quasi-separated morphisms](../../../../../quasi-separated-morphism.md) and [locally of finite type](../../../../../locally-of-finite-type.md) gives the other hypotheses of (a)(iii). Consequently

$$
\boxed{\begin{aligned}
f,g\text{ universally closed}&\Longrightarrow gf\text{ universally closed},\\
f,g\text{ separated}&\Longrightarrow gf\text{ separated},\\
f,g\text{ proper}&\Longrightarrow gf\text{ proper}.
\end{aligned}}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the introduction to schemes course of the University of Oxford](../../../../split.md)
6. [Introduction to schemes course of the University of Oxford](../../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
