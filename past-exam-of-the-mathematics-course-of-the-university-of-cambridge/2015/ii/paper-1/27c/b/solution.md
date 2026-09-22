<h1 id="27c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Near zero, write the amplitude as $t^{-1/4}(1+t)^{-1/4}=\sum_{m\geq0}\binom{-1/4}{m}t^{m-1/4}$. The large parameter localizes the integral at $t=0$. Termwise integration of the local expansion gives

$$
\int_0^\infty e^{-kt^2}t^{m-1/4}dt
=\frac12 k^{-3/8-m/2}\Gamma\left(\frac38+\frac m2\right).
$$

Consequently

$$
\boxed{\alpha=\frac38,\quad\beta=\frac12,\quad
a_m=\frac12\binom{-1/4}{m}\Gamma\left(\frac38+\frac m2\right)
=\frac{(-1)^m(1/4)_m}{2m!}\Gamma\left(\frac38+\frac m2\right)}.
$$

Here $(1/4)_m$ is the [rising factorial](../../../../../../rising-factorial.md). This is an asymptotic series, not an assertion that the full integrated Taylor series converges.

The needed result is [Watson's lemma](../../../../../../watson-s-lemma.md): if a locally integrable amplitude has an expansion $g(s)\sim\sum c_ms^{\rho_m-1}$ as $s\downarrow0$, with $\rho_m>0$ increasing and suitable growth at infinity so its Laplace integral converges, then $\int_0^\infty e^{-ks}g(s)ds\sim\sum c_m\Gamma(\rho_m)k^{-\rho_m}$, with the corresponding finite-order remainder bounds. Apply it after $s=t^2$, when $g(s)=\tfrac12s^{-5/8}(1+\sqrt s)^{-1/4}$ and $\rho_m=3/8+m/2$. The tail is exponentially small after any fixed positive cutoff.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27C](../../27c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
