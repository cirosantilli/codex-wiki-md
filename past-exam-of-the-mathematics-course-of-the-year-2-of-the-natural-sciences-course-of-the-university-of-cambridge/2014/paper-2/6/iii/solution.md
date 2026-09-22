<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An [axial vector](../../../../../pseudovector.md) transforms under an orthogonal matrix $Q$ as

$$
\boxed{a'_i=(\det Q)Q_{ij}a_j.}
$$

For a proper rotation, $\det Q=1$, so this is the usual [polar vector](../../../../../polar-vector.md) rule. Under an orientation-reversing change, the extra sign distinguishes the two. In particular, spatial inversion leaves an axial vector unchanged while reversing a polar vector.

Let $C_i=(\nabla\times u)_i=\epsilon_{ijk}\partial_j u_k$. The determinant identity for the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) is

$$
\epsilon_{ijk}Q_{jp}Q_{kq}=(\det Q)Q_{ir}\epsilon_{rpq}.
$$

It follows by multiplying the three-index determinant identity by $Q_{ir}$ and using orthogonality. The derivative transformation from part (ii) then gives

$$
\boxed{C'_i=\epsilon_{ijk}Q_{jp}Q_{kq}\partial_pu_q=(\det Q)Q_{ir}C_r.}
$$

Hence the [curl](../../../../../curl.md) of a polar vector field is an axial vector field. The Levi-Civita determinant factor is exactly the extra sign required under reflections.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
