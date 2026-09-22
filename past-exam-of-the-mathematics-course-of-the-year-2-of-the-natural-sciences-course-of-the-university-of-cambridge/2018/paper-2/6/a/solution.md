<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Split the [Cartesian second-rank tensor](../../../../../cartesian-second-rank-tensor.md) into symmetric and antisymmetric parts:

$$
S_{ij}=\frac{T_{ij}+T_{ji}}2,\qquad A_{ij}=\frac{T_{ij}-T_{ji}}2.
$$

Define $u_k=\frac12\epsilon_{kij}T_{ij}$. The symmetric part contributes zero to this contraction. The [epsilon-delta identity](../../../../../contraction-of-two-levi-civita-symbols.md) then gives

$$
\epsilon_{ijk}u_k=\frac12\epsilon_{ijk}\epsilon_{klm}T_{lm}
=\frac12(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})T_{lm}
=\frac{T_{ij}-T_{ji}}2=A_{ij}.
$$

Therefore

$$
\boxed{T_{ij}=S_{ij}+\epsilon_{ijk}u_k,\qquad
S_{ij}=\frac{T_{ij}+T_{ji}}2,\qquad u_k=\frac12\epsilon_{kij}T_{ij}}.
$$

The symmetric part and the three independent antisymmetric components determine these quantities uniquely. Under proper rotations $u$ is a [vector](../../../../../vector.md); under reflections it is an [axial vector](../../../../../pseudovector.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
