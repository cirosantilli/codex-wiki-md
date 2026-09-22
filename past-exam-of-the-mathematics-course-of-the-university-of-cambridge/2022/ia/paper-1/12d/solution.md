<h1 id="12d/solution">Solution</h1>

↑ **Parent:** [12D](../12d.md)

It is enough to treat an increasing function; replacing $f$ by $-f$ handles a decreasing one. Let $\mathcal R$ be the common refinement of dissections $\mathcal D$ and $\mathcal D'$. Refinement raises lower [Darboux sums](../../../../../darboux-sum.md) and lowers upper ones, so

$$
L_{\mathcal D}(f)\leq L_{\mathcal R}(f)
\leq U_{\mathcal R}(f)\leq U_{\mathcal D'}(f).
$$

For the uniform dissection $\mathcal D_n=\{k/n:0\leq k\leq n\}$, monotonicity gives the telescoping difference

$$
U_{\mathcal D_n}(f)-L_{\mathcal D_n}(f)
=\frac1n\sum_{k=1}^n
\left(f\left(\frac kn\right)-f\left(\frac{k-1}{n}\right)\right)
=\frac{f(1)-f(0)}n.
$$

This can be made smaller than any $\varepsilon>0$, so the [Riemann integrability criterion](../../../../../riemann-integrability-criterion.md) proves that $f$ is integrable.

The integral lies between the lower and upper sums, and the displayed sum in the question is the right-endpoint upper sum. Hence the generally valid sharp estimate is

$$
\boxed{
\left|\int_0^1f(x)\,dx
-\frac1n\sum_{k=1}^nf\left(\frac kn\right)\right|
\leq\frac{|f(1)-f(0)|}{n}}. \qquad (1)
$$

The strict inequality printed in the question is false for arbitrary monotone functions: if $f(x)=0$ for $x<1$ and $f(1)=1$, the two sides of (1) are both $1/n$.

For the final claim, write

$$
\Delta_n
=\sum_{k=1}^n\int_{(k-1)/n}^{k/n}
\left(F(x)-F\left(\frac kn\right)\right)dx.
$$

Since $F'$ is continuous on a compact interval, it is uniformly continuous. Uniformly for $0\leq t\leq1$,

$$
F\left(\frac{k-1+t}{n}\right)-F\left(\frac kn\right)
=-\frac{1-t}{n}F'\left(\frac kn\right)+o\left(\frac1n\right).
$$

After the substitution $x=(k-1+t)/n$, summing the uniform errors gives

$$
\Delta_n
=-\frac1{2n^2}\sum_{k=1}^nF'\left(\frac kn\right)
+o\left(\frac1n\right).
$$

The right-hand sum is a [Riemann integral](../../../../../riemann-integral.md), so the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) yields

$$
\lim_{n\to\infty}n\Delta_n
=-\frac12\int_0^1F'(x)\,dx
=\boxed{\frac{F(0)-F(1)}2}.
$$

## ↑ Ancestors (10)

1. [12D](../12d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
