<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For horizontal forcing the exact angular equation is

$$
\ddot\theta=-\frac gl\sin\theta+\frac{a\omega^2}{l}\cos\theta\cos\omega t.
$$

Write $\theta=\Theta+\xi$ with $\Theta=\theta_1$ slowly varying and $\xi=-(a/l)\cos\Theta\cos\omega t$. To leading order in the slow-to-fast frequency ratio, $\ddot\xi=(a\omega^2/l)\cos\Theta\cos\omega t$, which balances the rapid forcing. Expand the right-hand side to first order in $\xi$:

$$
\ddot\Theta+\ddot\xi
=-\frac gl(\sin\Theta+\xi\cos\Theta)
+\frac{a\omega^2}{l}(\cos\Theta-\xi\sin\Theta)\cos\omega t.
$$

During one fast period treat $\Theta$ as fixed. The averages $\langle\xi\rangle$ and $\langle\cos\omega t\rangle$ vanish, whereas

$$
\langle\xi\cos\omega t\rangle=-\frac{a}{2l}\cos\Theta.
$$

The leading averaged equation is therefore

$$
\boxed{\ddot\Theta=-\frac gl\sin\Theta+
\frac{a^2\omega^2}{2l^2}\sin\Theta\cos\Theta.}
$$

The effective force comes from correlation between the rapid displacement and the rapidly varying driving [torque](../../../../../torque.md); simply averaging the driving cosine to zero misses it. This keeps the leading nonzero fast-motion contribution, proportional to $a^2\omega^2$, while neglecting terms suppressed by additional powers of $a/l$ or of the slow rate divided by $\omega$. The gravitational expansion at order $g(a/l)^2$ is smaller in the stated high-frequency regime. The resulting slow frequencies must also remain small compared with $\omega$ for averaging to be self-consistent.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
