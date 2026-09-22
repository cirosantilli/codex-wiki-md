<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expanding the modulus squared yields an outgoing-angle factor $e^{-i\mathbf k_f\cdot\mathbf d}$ and an incoming factor $e^{i\mathbf k_i\cdot\mathbf d}$, where $\mathbf d=\mathbf r-\mathbf r'$. Choosing a polar axis along $\mathbf d$ gives

$$
\int d\Omega_f\,e^{-ik\widehat{\mathbf k}_f\cdot\mathbf d}
=2\pi\int_{-1}^1e^{-ikdu}\,du=4\pi\frac{\sin kd}{kd}.
$$

Consequently

$$
\boxed{\sigma^{(1)}_{\rm total}=\frac{m^2}{\pi\hbar^4}
\int d^3r\,d^3r'\,V(\mathbf r)V(\mathbf r')
\frac{\sin kd}{kd}\,e^{i\mathbf k_i\cdot\mathbf d}}.
$$

The apparent $d=0$ singularity is removable: $\sin(kd)/(kd)\to1$. Exchanging $\mathbf r$ and $\mathbf r'$ cancels the imaginary part, while nonnegativity follows directly from its origin as an integral of $|f^{(1)}|^2$. A complex absorbing potential would require $V(\mathbf r')^*$ instead; the lossless [optical theorem](../../../../../optical-theorem.md) comparison below uses real $V$.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
