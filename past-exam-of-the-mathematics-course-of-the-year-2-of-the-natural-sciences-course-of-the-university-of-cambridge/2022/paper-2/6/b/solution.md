<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $s=A_iA_i>0$, $q=A_iT_{ij}A_j$ and $\tau=T_{ii}$. Taking the [trace](../../../../../matrix-trace.md) of the proposed decomposition gives

$$
\tau=3\alpha+\beta s,
$$

since $A_iB_i=0$ and $C_{ii}=0$. Contracting twice with $A$ gives $q=\alpha s+\beta s^2$. Solving these two scalar equations yields

$$
\boxed{\alpha=\frac12\left(\tau-\frac qs\right),\qquad
\beta=\frac{3q-s\tau}{2s^2}.}
$$

A single contraction gives $T_{ij}A_j=(\alpha+\beta s)A_i+sB_i$, and $\alpha+\beta s=q/s$. Hence

$$
\boxed{B_i=\frac{T_{ij}A_j}{s}-\frac{qA_i}{s^2}.}
$$

Finally set

$$
\boxed{C_{ij}=T_{ij}-\alpha\delta_{ij}-\beta A_iA_j-B_iA_j-B_jA_i.}
$$

This is manifestly symmetric. The formulas give $A_iB_i=q/s-q/s=0$; substituting them into $C_{ij}A_j$ gives zero, and taking the [trace](../../../../../matrix-trace.md) gives $C_{ii}=0$. Since $C$ is symmetric, $A_iC_{ij}=0$ also holds.

A geometric form makes the [axis decomposition of a symmetric matrix](../../../../../axis-decomposition-of-a-symmetric-matrix.md) explicit. With the transverse [orthogonal projection](../../../../../orthogonal-projection.md) $P_{ij}=\delta_{ij}-A_iA_j/s$,

$$
B_i=\frac{P_{ij}T_{jk}A_k}{s},\qquad
C_{ij}=P_{ik}T_{kl}P_{lj}-\alpha P_{ij}.
$$

Here $\alpha$ is half the transverse [trace](../../../../../matrix-trace.md) and $C$ is its [symmetric traceless rank-two tensor](../../../../../symmetric-trace-free-square-of-the-defining-orthogonal-representation.md) part. Every term was forced by contractions, so the decomposition is unique.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
