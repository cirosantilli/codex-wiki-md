<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathfrak q$ be a [prime ideal](../../../../../../prime-ideal.md) of $C$. Its [quotient ring](../../../../../../quotient-ring.md) $D=C/\mathfrak q$ is a nonzero [integral domain](../../../../../../integral-domain.md) and a finite-dimensional $K$-vector space. For $0\ne a\in D$, multiplication by $a$ is an [injective](../../../../../../injective-function.md) $K$-linear map $D\to D$, because $D$ has no zero divisors. An [injective](../../../../../../injective-function.md) [endomorphism](../../../../../../endomorphism.md) of a [finite-dimensional vector space](../../../../../../finite-dimensional-vector-space.md) is [surjective](../../../../../../surjective-function.md). In particular $ab=1$ for some $b\in D$. Every nonzero element is therefore invertible, so $D$ is a [field](../../../../../../field.md) and $\mathfrak q$ is a [maximal ideal](../../../../../../maximal-ideal.md).

To prove finiteness, select any $r$ distinct [maximal ideals](../../../../../../maximal-ideal.md) $\mathfrak m_1,\ldots,\mathfrak m_r$. Distinct [maximal ideals](../../../../../../maximal-ideal.md) are comaximal: $\mathfrak m_i+\mathfrak m_j$ strictly contains $\mathfrak m_i$, so must equal $C$. The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) gives a [surjection](../../../../../../surjective-function.md)

$$
C\longrightarrow\prod_{i=1}^rC/\mathfrak m_i.
$$

Here is the needed surjectivity explicitly. For each $j\ne i$, choose $a_{ij}\in\mathfrak m_j$ with $a_{ij}\equiv1\pmod{\mathfrak m_i}$, using comaximality. Then $e_i=\prod_{j\ne i}a_{ij}$ is one modulo $\mathfrak m_i$ and zero modulo the other selected [ideals](../../../../../../ideal.md). Given any residue tuple represented by $b_i$, the element $\sum_i b_ie_i$ maps to that tuple. Thus the displayed map really is [surjective](../../../../../../surjective-function.md).

Each nonzero [field](../../../../../../field.md) quotient has $K$-dimension at least one, so

$$
r\leq\sum_{i=1}^r\dim_K(C/\mathfrak m_i)\leq\dim_KC.
$$

There cannot be more than $\dim_KC$ [maximal ideals](../../../../../../maximal-ideal.md), because otherwise one could select a finite list exceeding this bound. Consequently

$$
\boxed{\operatorname{Spec}C=\operatorname{MaxSpec}C,\qquad |\operatorname{MaxSpec}C|\leq\dim_KC<\infty.}
$$

This proves the description of the [spectrum of a finite-dimensional commutative algebra](../../../../../../spectrum-of-a-finite-dimensional-commutative-algebra.md). If $C=0$, its spectrum is empty and the same conclusion holds.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
