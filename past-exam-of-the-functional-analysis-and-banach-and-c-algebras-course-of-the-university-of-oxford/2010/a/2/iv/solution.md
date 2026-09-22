<h1 id="a/2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Define a [diagonal operator on sequence space](../../../../../diagonal-operator-on-sequence-space.md) by

$$
\boxed{S:c_0\longrightarrow\ell_2,\qquad Sx=(2^{-n}x_n)_{n\geq1}.}
$$

It is bounded because $\|Sx\|_2^2\leq\|x\|_\infty^2\sum_{n\geq1}4^{-n}=\|x\|_\infty^2/3$. Its truncation $S_mx=(2^{-1}x_1,\ldots,2^{-m}x_m,0,\ldots)$ is a [finite-rank operator](../../../../../finite-rank-operator.md), and

$$
\|S-S_m\|=\left(\sum_{n>m}4^{-n}\right)^{1/2}=\frac{2^{-m}}{\sqrt3}\longrightarrow0.
$$

Equality follows by using [finitely supported sequences](../../../../../finitely-supported-sequence.md) equal to $1$ on longer and longer finite tails. An [operator norm](../../../../../operator-norm.md) limit of [compact operators](../../../../../compact-operator-split.md) into the [Banach space](../../../../../banach-space-split.md) $\ell_2$ is compact; therefore **$S$ is a [compact operator](../../../../../compact-operator-split.md)**. The vectors $Se_n=2^{-n}e_n$ are [linearly independent](../../../../../linear-independence.md), so its rank is infinite.

There is no conflict with the preceding result about a compact closed-ball [image](../../../../../image-of-a-function.md). Indeed, take $x^{(m)}=(1,\ldots,1,0,\ldots)$ with $m$ initial ones. Then $Sx^{(m)}\to(2^{-n})_{n\geq1}$ in $\ell_2$, but that limit has no preimage in $c_0$: its only possible preimage is the constant sequence $1$. Thus $S(B_{c_0})$ is relatively compact but is not closed and hence is not compact.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
