<h1 id="1/iii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We prove (c)$\Rightarrow$(a) by induction on dimension. It suffices to work on an integral [projective variety](../../../../../../../projective-variety.md) $V$. By induction, $D$ is [ample](../../../../../../../ample-line-bundle.md) on every lower-dimensional integral [subvariety](../../../../../../../closed-subvariety.md), and hence on every lower-dimensional closed subscheme by [ampleness on reduced components](../../../../../../../ampleness-on-reduced-components.md).

Apply (c) to $V$ itself. The nonzero section of $\mathcal O_V(mD)$ has a nonempty zero divisor $E$. Because $V$ is integral, this is an [effective Cartier divisor](../../../../../../../effective-cartier-divisor.md) and $\mathcal O_V(E)\cong\mathcal O_V(mD)$. Its support has dimension less than $\dim V$, so $D|_E$, and therefore $\mathcal O_E(E)$, is [ample](../../../../../../../ample-line-bundle.md). Part (ii) makes $E$ [semiample](../../../../../../../semiample-divisor.md), hence some positive multiple of $D$ is [basepoint-free](../../../../../../../basepoint-free-divisor.md).

Let $f:V\to Y\subset\mathbb P^N$ be the resulting [Kodaira map](../../../../../../../kodaira-map.md), with $\mathcal O_V(qD)=f^*\mathcal O_Y(1)$. No fibre can have positive dimension: such a projective fibre contains an integral [projective curve](../../../../../../../projective-curve.md) $C$, on which $D$ has degree zero. But the assumed nonzero section of some $\mathcal O_C(rD)$ cannot vanish anywhere, since its nonempty [effective divisor](../../../../../../../effective-cartier-divisor.md) would have positive degree. This contradicts (c).

Thus $f$ has zero-dimensional fibres. A proper [quasi-finite morphism](../../../../../../../quasi-finite-morphism.md) is a [finite morphism](../../../../../../../finite-morphism.md). The [finite pullback of an ample line bundle](../../../../../../../finite-pullback-of-an-ample-line-bundle.md) is [ample](../../../../../../../ample-line-bundle.md), so $qD$ and then $D$ are [ample](../../../../../../../ample-line-bundle.md). This proves

$$
\boxed{\text{(c)}\Longrightarrow\text{(a)};\qquad\text{(a), (b), (c) are equivalent}.}
$$

The fibre argument proves the [semiample and curve-positive ampleness criterion](../../../../../../../semiample-and-curve-positive-ampleness-criterion.md). It also explains why testing only existence of a nonzero section, without requiring a zero, would be insufficient: the trivial bundle on a positive-dimensional [projective variety](../../../../../../../projective-variety.md) has a nowhere-vanishing section.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Iii](../../iii.md)
3. [1](../../../1.md)
4. [Paper 134](../../../../paper-134-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
