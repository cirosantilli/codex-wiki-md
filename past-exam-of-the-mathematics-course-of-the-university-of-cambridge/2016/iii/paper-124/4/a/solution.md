<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expand the two [Dirichlet polynomials](../../../../../../dirichlet-polynomial.md), keeping the [complex conjugate](../../../../../../complex-conjugate.md) on $B$. The diagonal $m=n$ contributes exactly $T\sum_{n\le X}a_n\overline{b_n}/n^{2\sigma}$. If $m\ne n$, the exponential integral is

$$
\int_T^{2T}e^{it\log(m/n)}\,dt=\frac{e^{2iT\log(m/n)}-e^{iT\log(m/n)}}{i\log(m/n)},
$$

whose absolute value is at most $2/|\log(m/n)|$. Thus **the mean-value formula** is

$$
\boxed{\int_T^{2T}A(\sigma+it)\overline{B(\sigma+it)}\,dt=T\sum_{n\le X}\frac{a_n\overline{b_n}}{n^{2\sigma}}+O\left(\sum_{\substack{m,n\le X\\m\ne n}}\frac{|a_n||b_m|}{n^\sigma m^\sigma|\log(m/n)|}\right).}
$$

This also covers $T=0$.

For $m>n$, integration of $1/x$ over $[n,m]$ gives $\log(m/n)\ge(m-n)/m$; the analogous inequality holds with $m,n$ exchanged. Hence $|\log(m/n)|^{-1}\le\max(m,n)/|m-n|\le X$. This gives the requested first bound $O\bigl(X\sum_{m\ne n}|a_n||b_m|/(n^\sigma m^\sigma)\bigr)$.

For the weighted bound, put $\alpha_n=|a_n|n^{-\sigma}$ and $\beta_m=|b_m|m^{-\sigma}$. The inequality

$$
2\alpha_n\beta_m\le\frac nm\alpha_n^2+\frac mn\beta_m^2
$$

reduces the estimate to a row sum and its symmetric counterpart. For a fixed $n$, the preceding logarithm bounds give

$$
\sum_{\substack{m\le X\\m\ne n}}\frac{n/m}{|\log(m/n)|}\le\sum_{m>n}\frac n{m-n}+\sum_{m<n}\frac{n^2}{m(n-m)}\ll n\log(2X).
$$

Here $n^2/(m(n-m))=n(1/m+1/(n-m))$, and each resulting [harmonic sum](../../../../../../harmonic-sum.md) is $O(\log(2X))$. The symmetric row sum is bounded by $O(m\log(2X))$. Therefore **the second error bound** is

$$
\boxed{O\left(\sum_{n\le X}\frac{|a_n|^2n\log(2X)}{n^{2\sigma}}+\sum_{m\le X}\frac{|b_m|^2m\log(2X)}{m^{2\sigma}}\right).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
