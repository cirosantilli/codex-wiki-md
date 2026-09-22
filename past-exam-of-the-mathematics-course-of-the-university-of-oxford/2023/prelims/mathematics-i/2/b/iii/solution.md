<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

If $T'=\lambda T$ with $\lambda\ne0$, then $T'(x)=0$ if and only if $T(x)=0$, so their [kernels](../../../../../../../kernel-of-a-linear-map-split.md) agree. Conversely, suppose both nonzero [linear functionals](../../../../../../../linear-functional.md) have [kernel](../../../../../../../kernel-of-a-linear-map-split.md) $K$. Choose $u$ with $T(u)=1$, by scaling a [vector](../../../../../../../vector.md) on which $T$ is nonzero. For each $x\in V$,

$$
x=T(x)u+\bigl(x-T(x)u\bigr),\qquad x-T(x)u\in K.
$$

Therefore $T'(x)=T(x)T'(u)$. Moreover $T'(u)\ne0$, since $u\notin K$. Thus $\boxed{T'=T'(u)T}$, with a nonzero [scalar](../../../../../../../scalar.md).

Every nonzero [linear functional](../../../../../../../linear-functional.md) $V\to\mathbb F_p$ is surjective, so its [kernel](../../../../../../../kernel-of-a-linear-map-split.md) has [dimension](../../../../../../../dimension-vector-space.md) $n-1$ by the [rank-nullity theorem](../../../../../../../rank-nullity-theorem.md). Conversely, every [hyperplane](../../../../../../../hyperplane.md) $K$ is such a [kernel](../../../../../../../kernel-of-a-linear-map-split.md): extend a [basis](../../../../../../../basis.md) of $K$ by one [vector](../../../../../../../vector.md) $u$, and assign value zero on that [basis](../../../../../../../basis.md) and value one on $u$. Hence the [hyperplanes](../../../../../../../hyperplane.md) containing $v$ are exactly the [kernels](../../../../../../../kernel-of-a-linear-map-split.md) of the $p^{n-1}-1$ nonzero [linear functionals](../../../../../../../linear-functional.md) counted above. Each [kernel](../../../../../../../kernel-of-a-linear-map-split.md) occurs for exactly $p-1$ of them, its distinct nonzero [scalar multiples](../../../../../../../scalar-multiple.md). The required number is

$$
\boxed{\frac{p^{n-1}-1}{p-1}.}
$$

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [b](../../b.md)
3. [2](../../../2.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
