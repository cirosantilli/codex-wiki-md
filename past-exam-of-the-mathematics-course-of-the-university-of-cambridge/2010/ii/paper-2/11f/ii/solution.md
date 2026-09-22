<h1 id="11f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose first that a [retraction](../../../../../../retraction.md) $R:D\to C$ exists. The [continuous map](../../../../../../continuous-map.md) $p\mapsto-R(p)$ takes $D$ to itself, so the [Brouwer fixed-point theorem](../../../../../../brouwer-fixed-point-theorem.md) gives $p=-R(p)$. Such $p$ lies on $C$, where $R(p)=p$, contradicting $p=-p$.

Conversely, suppose a [continuous map](../../../../../../continuous-map.md) $T:D\to D$ has no [fixed point](../../../../../../fixed-point.md). For each $p$, follow the ray from $T(p)$ through $p$ to its last intersection with $C$. This defines a [retraction](../../../../../../retraction.md). More explicitly, put $a=p-T(p)\ne0$ and set

$$
R(p)=T(p)+t(p)a,\qquad t(p)=\frac{-T(p)\cdot a+\sqrt{(T(p)\cdot a)^2+(1-|T(p)|^2)|a|^2}}{|a|^2}.
$$

The positive-root formula is continuous, $t(p)\geq1$, and $R(p)$ is on the unit circle. If $p\in C$, the last intersection is $p$ itself, so $R(p)=p$. Thus the nonexistence of a [retraction](../../../../../../retraction.md) rules out a fixed-point-free $T$, proving the equivalence.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
