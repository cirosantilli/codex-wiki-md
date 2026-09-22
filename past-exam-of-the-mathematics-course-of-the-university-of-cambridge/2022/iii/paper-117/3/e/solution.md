<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $M_0=CRT^2$ and split the last sum in part d according as $\tau_4(m)<X$ or $\tau_4(m)\geq X$. For the first part, the [reciprocal fractional-part sum near a rational](../../../../../../reciprocal-fractional-part-sum-near-a-rational.md) gives

$$
\sum_{\substack{m\leq M_0\\\tau_4(m)<X}}
\tau_4(m)\min(R,\|\alpha m\|^{-1})
\ll X(\log q)\left(\frac{M_0R}{q}+M_0+R+q\right).
$$

For the second part, use the supplied second-moment estimate and [truncation of a divisor weight by its second moment](../../../../../../truncation-of-a-divisor-weight-by-its-second-moment.md):

$$
\begin{aligned}
\sum_{\substack{m\leq M_0\\\tau_4(m)\geq X}}
\tau_4(m)\min(R,\|\alpha m\|^{-1})
&\leq R\sum_{\substack{m\leq M_0\\\tau_4(m)\geq X}}\tau_4(m)\\
&\ll\frac{RM_0}{X}(\log M_0)^{O(1)}.
\end{aligned}
$$

Substitute $M_0\asymp RT^2$, take fourth roots, and factor out $R^{1/2}T^{1/2}$. The four terms from the bounded-weight estimate become, after harmless enlargement by $(\log q)(\log RT)^{O(1)}$,

$$
\frac{X^{1/4}}{q^{1/4}},qquad
\frac{X^{1/4}}{R^{1/4}},qquad
\frac{X^{1/4}q^{1/4}}{R^{1/2}T^{1/2}},
$$

with the smaller $XR$ term absorbed by $XM_0$. The large-weight part contributes $X^{-1/4}$. Finally, the two diagonal terms from part d contribute $R^{-1/4}$ and $T^{-1/4}$; since $X\geq1$, the first is absorbed by $X^{1/4}R^{-1/4}$. Therefore

$$
\boxed{
|S|\ll\|b\|_2\|c\|_2(\log q)(\log RT)^{O(1)}R^{1/2}T^{1/2}
\left(
\frac1{X^{1/4}}+\frac{X^{1/4}}{q^{1/4}}
+\frac{X^{1/4}}{R^{1/4}}
+\frac{X^{1/4}q^{1/4}}{R^{1/2}T^{1/2}}
+\frac1{T^{1/4}}
\right).}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
