<h1 id="10/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $s_n(x)=\sin(q_nx)$ and $s_m(x)=\sin(q_mx)$. Their [differential equations](../../../../../differential-equation-split.md) are $-s_n''=q_n^2s_n$ and $-s_m''=q_m^2s_m$. Subtract the two cross-multiplied equations and use [integration by parts](../../../../../integration-by-parts.md):

$$
(q_n^2-q_m^2)\int_0^1s_ns_m\,dx=[s_ns_m'-s_ms_n']_0^1.
$$

The lower boundary term is zero because both functions vanish there. At the upper endpoint, the [Robin boundary condition](../../../../../robin-boundary-condition.md) gives $s_j'(1)=s_j(1)/\alpha$, so

$$
s_n(1)s_m'(1)-s_m(1)s_n'(1)=\frac{s_n(1)s_m(1)}\alpha-\frac{s_m(1)s_n(1)}\alpha=0.
$$

Since distinct positive roots have $q_n^2\ne q_m^2$, we conclude

$$
\boxed{\int_0^1\sin(q_nx)\sin(q_mx)\,dx=0,\qquad n\ne m.}
$$

This [orthogonality](../../../../../orthogonal-vectors.md) holds for every $\alpha>0$, even when the sine family requires the additional nonpositive mode for completeness as explained in part (c).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
