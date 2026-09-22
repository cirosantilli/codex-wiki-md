<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The map $T\mapsto T^{\mathsf T}A+AT$ is linear, so its [kernel](../../../../../../kernel-of-a-linear-map.md) $L$ is a [vector subspace](../../../../../../vector-subspace.md) of the [matrix algebra](../../../../../../matrix-algebra.md). If $T_1,T_2\in L$, use $T_i^{\mathsf T}A=-AT_i$ to compute

$$
\begin{aligned}
[T_1,T_2]^{\mathsf T}A
&=(T_2^{\mathsf T}T_1^{\mathsf T}-T_1^{\mathsf T}T_2^{\mathsf T})A\\
&=-T_2^{\mathsf T}AT_1+T_1^{\mathsf T}AT_2\\
&=AT_2T_1-AT_1T_2=-A[T_1,T_2].
\end{aligned}
$$

Thus $L$ is closed under the [commutator](../../../../../../commutator.md). This bracket is bilinear and satisfies $[T,T]=0$. Associativity of matrix multiplication gives the [Jacobi identity](../../../../../../jacobi-identity.md): expanding $[T_1,[T_2,T_3]]+[T_2,[T_3,T_1]]+[T_3,[T_1,T_2]]$ makes each of the six ordered triple products occur once with each sign. Therefore **$L$ is a Lie algebra**. No nonsingularity or symmetry assumption on $A$ was needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
