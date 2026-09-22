<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $n\geq1$ put $C_n=\overline{T(n\overline B_X)}$, with [closure](../../../../../closure-topology.md) taken in $Y$. Then

$$
T(X)=\bigcup_{n=1}^{\infty}T(n\overline B_X)\subseteq\bigcup_{n=1}^{\infty}C_n.
$$

If every $C_n$ has empty [interior](../../../../../interior-topology.md), then each $C_n$ is a [nowhere dense set](../../../../../nowhere-dense-set.md), because it is closed. Each $T(n\overline B_X)$ is then a [nowhere dense set](../../../../../nowhere-dense-set.md) too. Consequently $T(X)$ is a [meagre set](../../../../../meagre-set.md), that is, a set of the first category in $Y$.

Otherwise some $C_n$ has nonempty [interior](../../../../../interior-topology.md). Scaling gives nonempty [interior](../../../../../interior-topology.md) of $\overline{T(\overline B_X)}$. The [geometric correction for approximate surjectivity](../../../../../geometric-correction-for-approximate-surjectivity.md) proved in the preceding part gives an open [ball](../../../../../ball-mathematics.md) about zero inside $T(\overline B_X)$. Since $T(X)$ is a [vector subspace](../../../../../vector-subspace.md), it then equals $Y$: scale any $y\in Y$ into this [ball](../../../../../ball-mathematics.md) and scale its preimage back. Hence $T(X)$ is a [closed set](../../../../../closed-set.md).

Thus, in fact, the stronger [operator range category dichotomy](../../../../../operator-range-category-dichotomy.md) holds:

$$
\boxed{T(X)=Y\quad\text{or}\quad T(X)\text{ is meagre in }Y.}
$$

In particular $T(X)$ is closed or of the first category, as required. The only substantive theorem used here is the preceding [geometric correction for approximate surjectivity](../../../../../geometric-correction-for-approximate-surjectivity.md): for a [bounded linear operator](../../../../../continuous-linear-operator.md) from a [Banach space](../../../../../banach-space-split.md) to a [normed space](../../../../../normed-vector-space-split.md), nonempty [interior](../../../../../interior-topology.md) of the closure of the image of the [unit ball](../../../../../unit-ball.md) implies nonempty [interior](../../../../../interior-topology.md) of the image itself. Its series proof was given there, so this proof does not require the [Baire category theorem](../../../../../baire-category-theorem.md) or completeness of $Y$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
