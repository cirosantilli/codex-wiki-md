<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $T_{\theta,\mathbf b}(\mathbf v)=R_\theta\mathbf v+\mathbf b$. The [sine addition formula](../../../../../../../sine-addition-formula.md) and [cosine addition formula](../../../../../../../cosine-addition-formula.md) give $R_\theta R_\psi=R_{\theta+\psi}$. Therefore [function composition](../../../../../../../function-composition.md) satisfies

$$
T_{\theta,\mathbf b}\circ T_{\psi,\mathbf c}=T_{\theta+\psi,\,R_\theta\mathbf c+\mathbf b}.
$$

The resulting [angle](../../../../../../../angle.md) is real and the new [translation](../../../../../../../translation-geometry.md) [vector](../../../../../../../vector.md) lies in $\mathbb R^2$, so $G$ is closed under [function composition](../../../../../../../function-composition.md). [Associativity](../../../../../../../associative-property.md) holds because, for any [functions](../../../../../../../function-split.md) $S,T,U$ and any $\mathbf v$, both $(S\circ T)\circ U$ and $S\circ(T\circ U)$ take $\mathbf v$ to $S(T(U(\mathbf v)))$.

The [identity element](../../../../../../../identity-element.md) is $T_{0,\mathbf0}$, since $R_0=I$. Every element has the two-sided [inverse element](../../../../../../../inverse-element.md)

$$
\boxed{T_{\theta,\mathbf b}^{-1}=T_{-\theta,\,-R_{-\theta}\mathbf b}.}
$$

Indeed $R_\theta R_{-\theta}=R_{-\theta}R_\theta=I$, and substituting into the composition formula makes the [translation](../../../../../../../translation-geometry.md) [vector](../../../../../../../vector.md) zero in either order. These verify all the [group axioms](../../../../../../../group-axioms.md). Thus **$G$ is a [group](../../../../../../../group-split.md) under [function composition](../../../../../../../function-composition.md)**, the [special Euclidean group](../../../../../../../special-euclidean-group.md) in two dimensions.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Mathematics IV resit](../../../../mathematics-iv-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
