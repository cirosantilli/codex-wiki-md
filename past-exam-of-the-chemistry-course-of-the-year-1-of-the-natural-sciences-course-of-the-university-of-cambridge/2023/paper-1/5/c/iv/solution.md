<h1 id="5/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $r_i$ be the event rate for step $i$, so

$$
r_1=k_1[\mathrm M][\mathrm{Cl_2}],\quad
r_2=k_2[\mathrm{Cl}][\mathrm{H_2}],\quad
r_3=k_3[\mathrm H][\mathrm{Cl_2}],\quad
r_4=k_4[\mathrm{Cl}]^2[\mathrm M].
$$

The [free radical](../../../../../../radical-chemistry.md) balances, including the factors of two for initiation and termination, are

$$
\begin{aligned}
0&\simeq r_2-r_3,\\
0&\simeq2r_1-r_2+r_3-2r_4.
\end{aligned}
$$

Thus $r_2=r_3$ and $r_1=r_4$, giving

$$
[\mathrm{Cl}]=\sqrt{\frac{k_1[\mathrm{Cl_2}]}{k_4}},\qquad
[\mathrm H]=\frac{k_2[\mathrm{Cl}][\mathrm{H_2}]}{k_3[\mathrm{Cl_2}]}.
$$

Both propagation events form [hydrogen chloride](../../../../../../hydrogen-chloride.md), so

$$
\boxed{\frac{\mathrm d[\mathrm{HCl}]}{\mathrm dt}
=2k_2\sqrt{\frac{k_1}{k_4}}[\mathrm{H_2}][\mathrm{Cl_2}]^{1/2}.}
$$

**The orders are one in [hydrogen](../../../../../../hydrogen.md), one half in [chlorine](../../../../../../chlorine.md) and three halves overall**, with $k_{\rm obs}=2k_2\sqrt{k_1/k_4}$ when the observed rate is HCl formation. If the rate is instead defined as the stoichiometrically normalized reaction rate, half that formation rate, the prefactor lacks the factor two. The bath [concentration](../../../../../../concentration.md) cancels because the same M-assisted initiation and recombination control the [free radical](../../../../../../radical-chemistry.md) pool. The result does not require $k_2=k_3$; different [free radical](../../../../../../radical-chemistry.md) concentrations make their steady fluxes equal. For molar [concentration](../../../../../../concentration.md), $k_{\rm obs}$ has units $\mathrm{dm^{3/2}\,mol^{-1/2}\,s^{-1}}$.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the chemistry course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Chemistry course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
