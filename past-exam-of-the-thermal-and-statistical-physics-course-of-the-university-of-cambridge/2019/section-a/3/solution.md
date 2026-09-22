<h1 id="section-a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the classical dilute-gas convention

$$
\frac{p}{nk_BT}=1+B_2(T)n+O(n^2),
$$

so the [second virial coefficient](../../../../second-virial-coefficient.md) has units of [volume](../../../../volume-thermodynamics.md). The [Mayer f-function](../../../../mayer-f-function.md) formula for an isotropic [pair potential](../../../../pair-potential.md) is

$$
B_2(T)=2\pi\int_0^\infty[1-e^{-\beta\phi(r)}]r^2\,dr.
$$

Only separations smaller than $a$ contribute. Define $x=\beta\varepsilon>0$ and substitute $t=r^3/a^3$, so $r^2dr=(a^3/3)dt$:

$$
B_2(T)=\frac{2\pi a^3}{3}\int_0^1[1-e^{-x(1-t)}]dt
=\boxed{\frac{2\pi a^3}{3}\left[1-\frac{1-e^{-x}}x\right],\qquad x=\frac{\varepsilon}{k_BT}.}
$$

This is the [second virial coefficient of a bounded cubic repulsion](../../../../second-virial-coefficient-of-a-bounded-cubic-repulsion.md). For every finite positive $T$, $1-e^{-x}<x$, so $B_2(T)>0$. There is no finite positive [Boyle temperature](../../../../boyle-temperature.md). At high [temperature](../../../../temperature-split.md), expanding the exponential gives

$$
B_2(T)=\frac{2\pi a^3}{3}\left(\frac x2-\frac{x^2}{6}+O(x^3)\right)
\sim\frac{\pi a^3\varepsilon}{3k_BT}\longrightarrow0^+.
$$

Thus the intended limiting statement is

$$
\boxed{T_B=+\infty\quad\text{in the sense that }B_2(T)\to0\text{ only as }T\to\infty.}
$$

At the other extreme the classical expression tends to $2\pi a^3/3$, the hard-exclusion value for separation $a$. This is a check on the [integral](../../../../integral-split.md), not a claim that a real molecular gas stays classical at arbitrarily low [temperature](../../../../temperature-split.md). A molar [virial expansion](../../../../virial-expansion.md) would instead use $B_{2,\mathrm m}=N_A B_2$.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Section A](../../section-a.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
