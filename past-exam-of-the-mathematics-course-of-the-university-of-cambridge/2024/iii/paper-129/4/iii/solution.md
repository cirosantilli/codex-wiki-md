<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $s\in\mathbb F_p^n$, let

$$
r(s)=|\{(a,c)\in A^2:a+c=s\}|.
$$

The number $T$ of ordered three-term [arithmetic progressions](../../../../../../arithmetic-progression.md) in $A$ is

$$
T=\sum_{b\in A}r(2b).
$$

By the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md),

$$
T^2\le |A|\sum_{b\in A}r(2b)^2
\le |A|\sum_s r(s)^2.
$$

The last sum is the [additive energy](../../../../../../additive-energy.md) of $A$, namely the number of [additive quadruples](../../../../../../additive-quadruple.md). If $T\ge\eta|A|^2$, then

$$
\boxed{E(A)\ge T^2/|A|\ge\eta^2|A|^3.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
