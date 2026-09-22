<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Write $dm=dt/(2\pi)$ in angular coordinates on the unit circle. The centered [Hardy-Littlewood maximal function](../../../../../hardy-littlewood-maximal-function.md) is

$$
Mf(\omega)=\sup_{0<r\leq\pi}\frac1{m(I_r(\omega))}\int_{I_r(\omega)}|f|\,dm,
$$

where $I_r(\omega)$ is the centered circular arc of angular radius $r$, with $r=\pi$ giving the whole circle. The [Hardy-Littlewood maximal inequality](../../../../../hardy-littlewood-maximal-inequality.md) in this one-dimensional setting is the weak-type estimate

$$
\boxed{m\{Mf>\alpha\}\leq\frac3\alpha\|f\|_{L^1(m)}\qquad(\alpha>0).}
$$

The precise constant is not important for differentiation, but we prove this one explicitly.

Let $E=\{Mf>\alpha\}$ and choose a compact subset $F\subset E$. For each point of $F$, choose a centered arc whose average of $|f|$ exceeds $\alpha$. A finite subfamily covers $F$. Order these arcs by decreasing length and retain an arc precisely when it is disjoint from the previously retained arcs. Every rejected arc meets a retained arc of at least its length and lies in the latter's triple, interpreted on the circle and truncated to the whole circle if necessary. If the retained disjoint arcs are $I_1,\ldots,I_N$, then

$$
\begin{aligned}
m(F)&\leq\sum_{j=1}^N m(3I_j)
\leq3\sum_{j=1}^N m(I_j)\\
&<\frac3\alpha\sum_{j=1}^N\int_{I_j}|f|\,dm
\leq\frac3\alpha\|f\|_1.
\end{aligned}
$$

This is the interval version of the [Wiener covering lemma](../../../../../wiener-covering-lemma.md). The superlevel set is measurable: the average at each fixed radius is continuous in the center, by translation continuity in $L^1$, so $E$ is open. [Inner regularity of Lebesgue measure](../../../../../inner-regularity-of-lebesgue-measure.md) now passes the compact-set bound to $E$, proving the [Hardy-Littlewood maximal inequality](../../../../../hardy-littlewood-maximal-inequality.md). The same finite-interval argument gives the line version $|\{Mf>\alpha\}|\leq3\|f\|_1/\alpha$ for integrable functions on the real line.

To prove differentiation, first recall that continuous functions are dense in $L^1(m)$ on the circle. Approximate an integrable function by simple functions; for each of their measurable sets, inner and outer regularity give a compact subset and an open superset with arbitrarily small measure difference. A continuous cutoff between these sets approximates the indicator in $L^1$. Combining finitely many cutoffs proves the claimed density.

For a representative of $f$ finite almost everywhere, define its local absolute oscillation by

$$
\Delta f(\omega)=\limsup_{r\downarrow0}
\frac1{m(I_r(\omega))}\int_{I_r(\omega)}|f(\zeta)-f(\omega)|\,dm(\zeta).
$$

If $h$ is continuous and $u=f-h$, the triangle inequality and continuity of $h$ give

$$
\Delta f(\omega)\leq Mu(\omega)+|u(\omega)|.
$$

Thus the [Hardy-Littlewood maximal inequality](../../../../../hardy-littlewood-maximal-inequality.md) and the elementary integral bound for a superlevel set yield, for every $\varepsilon>0$,

$$
\begin{aligned}
m\{\Delta f>\varepsilon\}
&\leq m\{Mu>\varepsilon/2\}+m\{|u|>\varepsilon/2\}\\
&\leq\frac{8}{\varepsilon}\|f-h\|_1.
\end{aligned}
$$

Choose continuous $h$ with $\|f-h\|_1$ arbitrarily small. It follows that $\Delta f=0$ outside a null set, by using positive rational $\varepsilon$. In particular,

$$
\left|\frac1{m(I_r(\omega))}\int_{I_r(\omega)}f\,dm-f(\omega)\right|
\leq\frac1{m(I_r(\omega))}\int_{I_r(\omega)}|f-f(\omega)|\,dm\longrightarrow0
$$

for almost every $\omega$. This proves the requested [Lebesgue differentiation theorem](../../../../../lebesgue-differentiation-theorem.md), including the stronger absolute-oscillation formulation, rather than assuming pointwise convergence of the approximating continuous functions.

For failure at a specified point, use coordinates $-\pi<t\leq\pi$ and put $a_n=2^{-2^n}$. Let $f$ be one on the annuli $a_{2j+1}<|t|\leq a_{2j}$ for $j\geq0$, and zero elsewhere, including at zero. This bounded measurable function is integrable. Since $a_{n+1}/a_n\to0$, the average $A_n$ over the centered interval $[-a_n,a_n]$ satisfies

$$
1-\frac{a_{n+1}}{a_n}\leq A_n\leq1\quad(n\text{ even}),
\qquad
0\leq A_n\leq\frac{a_{n+1}}{a_n}\quad(n\text{ odd}).
$$

Indeed, the outermost annulus occupies all but the fraction $a_{n+1}/a_n$ of that interval, and has value one or zero according to parity. **The even-radius subsequence tends to one and the odd-radius subsequence to zero**, so no centered-average limit exists at $\omega=1$. The normalization of $m$ cancels from these averages. This is how [oscillating annuli obstruct differentiation at a point](../../../../../oscillating-annuli-obstruct-differentiation-at-a-point.md) without contradicting almost-everywhere differentiation.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
