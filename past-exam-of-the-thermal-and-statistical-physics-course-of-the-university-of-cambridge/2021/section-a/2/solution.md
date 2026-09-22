<h1 id="section-a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An additive-looking [energy](../../../../energy-split.md) expression does not by itself establish two [noninteracting subsystems](../../../../noninteracting-subsystems.md). Their allowed [microstates](../../../../microstate.md) must also form a [Cartesian product](../../../../cartesian-product.md) of independently available states. Here the second label's allowed values depend on the first. The four allowed pairs and their [energies](../../../../energy-split.md) are

$$
\begin{array}{c|c|c}
J&m_J&E/\epsilon\\\hline
1&-1&0\\
1&+1&2\\
2&-2&0\\
2&+2&4
\end{array}
$$

The [canonical partition function](../../../../canonical-partition-function.md), with $\beta=(k_BT)^{-1}$, is therefore

$$
Z=\sum_{J=1,2}e^{-\beta\epsilon J}\left(e^{\beta\epsilon J}+e^{-\beta\epsilon J}\right)
=\boxed{2+e^{-2\beta\epsilon}+e^{-4\beta\epsilon}.}
$$

The conditional sum over $m_J$ is $2\cosh(\beta\epsilon J)$ and depends on $J$; it cannot be pulled out as the [partition function](../../../../canonical-partition-function.md) of an independent second subsystem. Summing independently over $J\in\{1,2\}$ and all four values $m\in\{-2,-1,1,2\}$ would invent four forbidden pairs and give eight states instead of four.

One can make the state labels independent by writing $s=m_J/J=\pm1$, but then $E(J,s)=\epsilon J(1+s)$ contains a coupling between them. For genuinely additive independent [energies](../../../../energy-split.md), the difference between the $s=+1$ and $s=-1$ states would be independent of $J$; here it is $2\epsilon J$. Hence **the proposed $J$ and $m_J$ subsystems cannot be treated as noninteracting independent subsystems**. The literal two-value reading of the PDF's endpoint notation has been used. If that notation were instead intended as shorthand for full angular-momentum multiplets, including every integer between the endpoints, the eight allowed states would give

$$
Z_{\rm full}=2+2e^{-\beta\epsilon}+2e^{-2\beta\epsilon}+e^{-3\beta\epsilon}+e^{-4\beta\epsilon}.
$$

The conclusion about the failure of independent-subsystem factorization is unchanged. The two state-counting conventions should not be mixed.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
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
