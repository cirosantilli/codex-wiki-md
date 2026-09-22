<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $F(s)=-\zeta'(s)/\zeta(s)$. The [Euler product](../../../../../../euler-product.md) gives $F(s)=\sum_{n\geq1}\Lambda(n)n^{-s}$ for $\Re s>1$. The elementary nonnegative polynomial

$$
3+4\cos u+\cos2u=2(1+\cos u)^2
$$

therefore gives the [three-four-one zero-free-region argument](../../../../../../three-four-one-zero-free-region-argument.md):

$$
0\leq3F(\sigma)+4\Re F(\sigma+it)+\Re F(\sigma+2it)
\qquad(\sigma>1).
$$

The coefficients $\Lambda(n)$ are nonnegative; applying the identity with $u=t\log n$ justifies the inequality term by term.

Take real parts in the [global partial-fraction expansion of the zeta logarithmic derivative](../../../../../../global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative.md). For $1<\sigma\leq2$, the [digamma function](../../../../../../digamma-function.md) bounds yield

$$
\Re F(\sigma+it)
\leq\Re\frac1{\sigma+it-1}
-\sum_\rho\frac{\sigma-\beta}{(\sigma-\beta)^2+(t-\gamma)^2}
+C\log(|t|+2).
$$

All terms in the zero sum are nonnegative, because the [Euler product](../../../../../../euler-product.md) and completed [functional equation](../../../../../../functional-equation.md) locate the nontrivial zeros in the closed critical strip. The constant terms are bounded: in particular $\sum_\rho\Re(1/\rho)=\sum_\rho\beta/|\rho|^2$ converges. Near the real [pole](../../../../../../pole.md), $F(\sigma)=1/(\sigma-1)+O(1)$.

First exclude zeros on the line one. If $1+it$, $t\ne0$, were a zero of multiplicity $m\geq1$, the selected zero term would give

$$
\Re F(\sigma+it)\leq-\frac m{\sigma-1}+O_t(1),
\qquad \Re F(\sigma+2it)\leq O_t(1).
$$

Inserted into the positivity inequality, this yields $0\leq(3-4m)/(\sigma-1)+O_t(1)$, impossible as $\sigma\downarrow1$. At $t=0$, zeta has a [pole](../../../../../../pole.md), with a punctured neighbourhood containing no zeros. Thus the line one has no zeros.

Now let $\rho=\beta+i\gamma$ with $|\gamma|\geq1$ and put $L=\log(|\gamma|+2)$. Select this zero in the formula at $t=\gamma$ and discard every other nonnegative zero kernel. The [pole](../../../../../../pole.md) terms at heights $\gamma,2\gamma$ are bounded. Consequently

$$
0\leq\frac3{\sigma-1}-\frac4{\sigma-\beta}+C_1L.
$$

Choose a fixed positive $a$ small enough that $C_1a\leq1/2$ and $1+a/L\leq2$, and set $\sigma=1+a/L$, $h=1-\beta$. Rearranging gives

$$
\frac4{a/L+h}\leq L\left(\frac3a+C_1\right),\qquad
h\geq\frac{a(1-C_1a)}{(3+C_1a)L}\geq\frac a{7L}.
$$

This is the required logarithmic gap at large height.

For $|\gamma|\leq1$, zeros with $\beta\leq1/2$ already have a fixed gap. The remaining compact region contains finitely many zeros, none on the line one; the [pole](../../../../../../pole.md) at one cannot be an accumulation point of zeros. Hence those zeros also have a fixed positive distance from that line. Reduce the absolute constant to cover this bounded-height region and to make the preceding weak inequality strict. The [zero-free region of the Riemann zeta function](../../../../../../zero-free-region-of-the-riemann-zeta-function.md) is therefore

$$
\boxed{\beta<1-\frac{c}{\log(|\gamma|+2)}
\quad\text{for every nontrivial zero, with an absolute }c>0.}
$$

This proof has established boundary nonvanishing as well as the quantitative gap, rather than assuming the former implicitly.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
