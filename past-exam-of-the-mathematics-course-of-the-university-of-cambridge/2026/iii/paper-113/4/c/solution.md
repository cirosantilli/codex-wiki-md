<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $X=\operatorname{Spec}B$, $Y=\operatorname{Spec}A$, and let the morphism correspond to a homomorphism $\varphi:A\to B$. Put $I=\ker\varphi$ and

$$
Z=\operatorname{Spec}(A/I).
$$

The injection $A/I\hookrightarrow B$ gives $X\to Z$, and the quotient $A\to A/I$ gives a [closed immersion](../../../../../../closed-immersion.md) $Z\hookrightarrow Y$, so $f$ factors through $Z$.

If $f$ factors through another closed subscheme $Z'=\operatorname{Spec}(A/J)$, then $J\subseteq\ker\varphi=I$. The resulting quotient $A/J\to A/I$ induces the unique factorization $Z\to Z'\to Y$. Thus $Z$ is the [scheme-theoretic image](../../../../../../scheme-theoretic-image.md).

It remains to identify its underlying set. A [principal open subscheme](../../../../../../principal-open-subscheme.md) $D(a)\subseteq\operatorname{Spec}A$ misses $f(X)$ exactly when $D(\varphi(a))$ is empty, equivalently when $\varphi(a)$ is a [nilpotent element](../../../../../../nilpotent.md). Hence the ideal of functions vanishing set-theoretically on $f(X)$ has radical $\sqrt{\ker\varphi}$. The closure is therefore

$$
V(\sqrt{\ker\varphi})=V(\ker\varphi)=|Z|,
$$

as required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
