<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For proper rotations the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) is invariant, so contracting the two rank-one tensors $\partial_j$ and $v_k$ gives $c_i=\epsilon_{ijk}\partial_jv_k$ with transformation $c_i'=R_{i\ell}c_\ell$. Thus the [curl](../../../../../curl.md) is a vector under proper rotations. Under an orientation-reversing orthogonal change it acquires an additional determinant sign: it is an [axial vector](../../../../../pseudovector.md) when $v$ is a polar vector.

Commuting smooth partial derivatives and using epsilon contraction gives the [curl of the curl identity](../../../../../curl-of-the-curl-identity.md):

$$
[\nabla\times(\nabla\times v)]_i=\epsilon_{ijk}\epsilon_{klm}\partial_j\partial_lv_m=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j\partial_lv_m=\partial_i(\partial_jv_j)-\partial_j\partial_jv_i.
$$

Now take the curl of [Faraday's law](../../../../../faraday-s-law-of-induction.md) and use the vacuum [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md): $\nabla\times\nabla\times E=-\partial_t(\nabla\times B)=-c^{-2}E_{tt}$. Since $\nabla\cdot E=0$, the identity gives $\Delta E-c^{-2}E_{tt}=0$. Taking the curl of the [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md) gives the same result for $B$, using $\nabla\cdot B=0$. Hence both satisfy the [electromagnetic wave equation](../../../../../electromagnetic-wave-equation.md)

$$
\boxed{-\Delta E+c^{-2}E_{tt}=0,\qquad-\Delta B+c^{-2}B_{tt}=0.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
