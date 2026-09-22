<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [truncated Perron formula](../../../../../../truncated-perron-formula.md) says that if $F(s)=\sum_{n\geq1}a_nn^{-s}$ converges absolutely for $\Re s>\sigma_a$, then for $c>\sigma_a$, $T\geq2$, and $x$ not an integer,

$$
\sum_{n\leq x}a_n
=\frac1{2\pi i}\int_{c-iT}^{c+iT}F(s)\frac{x^s}{s}\,ds
+O\left(\sum_{n\geq1}|a_n|\left(\frac xn\right)^c
\min\left\{1,\frac1{T|\log(x/n)|}\right\}\right).
$$

Take $a_n=\Lambda(n)$ and $c=1+1/\log x$. The [logarithmic derivative](../../../../../../logarithmic-derivative.md) identity gives $F(s)=-\zeta'(s)/\zeta(s)$. Since $x-1/2$ is an integer, $|x-n|\geq1/2$ for every integer $n$. In the range $x/2<n<2x$,

$$
|\log(x/n)|\asymp\frac{|x-n|}{x},
$$

and hence the contribution there is

$$
\ll\frac{x\log x}{T}\sum_{x/2<n<2x}\frac1{|x-n|}
\ll\frac{x(\log x)^2}{T}.
$$

The ranges $n\leq x/2$ and $n\geq2x$ are bounded by the same quantity using absolute convergence and $-\zeta'(c)/\zeta(c)\ll\log x$. Therefore

$$
\boxed{\sum_{n\leq x}\Lambda(n)
=-\frac1{2\pi i}\int_{1+1/\log x-iT}^{1+1/\log x+iT}
\frac{\zeta'(s)}{\zeta(s)}\frac{x^s}{s}\,ds
+O\left(\frac{x(\log x)^2}{T}\right).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
