<h1 id="11d/solution">Solution</h1>

↑ **Parent:** [11D](../11d.md)

For a bounded real function on $[a,\infty)$, convergence of its [improper integral](../../../../../improper-integral.md) means that its restriction to every $[a,b]$, $b>a$, is [Riemann integrable](../../../../../riemann-integrable-function.md) and that the finite limit

$$
\boxed{\int_a^\infty f(x)\,dx
:=\lim_{b\to\infty}\int_a^b f(x)\,dx\in\mathbb R}
$$

exists. Boundedness by itself does not guarantee either local [Riemann integrability](../../../../../riemann-integrable-function.md) or existence of this limit.

A [monotone function](../../../../../monotonic-function.md) on $[a,b]$ is bounded between its endpoint values. Divide the interval into $m$ equal pieces with endpoints $x_j=a+j(b-a)/m$. If $f$ is nondecreasing, its upper and lower [Darboux sums](../../../../../darboux-sum.md) differ by

$$
U(f,P)-L(f,P)
=\frac{b-a}{m}\sum_{j=1}^m\bigl(f(x_j)-f(x_{j-1})\bigr)
=\frac{b-a}{m}\bigl(f(b)-f(a)\bigr).
$$

For nonincreasing $f$, the same calculation with reversed endpoint values gives $(b-a)(f(a)-f(b))/m$. Thus in either case $U-L=(b-a)|f(b)-f(a)|/m\to0$. For every $\varepsilon>0$ one can choose $m$ to make this gap smaller than $\varepsilon$; the [Riemann integrability criterion](../../../../../riemann-integrability-criterion.md) proves that $f$ is [Riemann integrable](../../../../../riemann-integrable-function.md).

Now let $f$ be decreasing on $[1,\infty)$ with limit zero. For each $x$, $f(x)\geq\lim_{y\to\infty}f(y)=0$. On $[n,n+1]$ its monotonicity gives

$$
f(n+1)\leq\int_n^{n+1}f(x)\,dx\leq f(n).
$$

Summing these bounds, with $S_N=\sum_{n=1}^Nf(n)$, yields

$$
\int_1^{N+1}f(x)\,dx\leq S_N
\leq f(1)+\int_1^Nf(x)\,dx.
$$

Both the [partial sums](../../../../../partial-sum.md) $S_N$ and the truncated integrals are nondecreasing because $f\geq0$. The inequalities show that one family is bounded above if and only if the other is. The [bounded monotone sequence theorem](../../../../../bounded-monotone-sequence-theorem.md) then gives convergence of the sums exactly when the integer-endpoint integrals converge. For real $b$ between $N$ and $N+1$, the integral to $b$ lies between the integrals to these integer endpoints; the [squeeze theorem](../../../../../squeeze-theorem.md) supplies the same limit. If either family is unbounded, both tend to $+\infty$. This proves the [integral test for convergence](../../../../../integral-test-for-convergence.md) in the required form.

For $\alpha<0$, use $f(x)=x^\alpha$, which is decreasing and tends to zero. Its truncated [improper integral](../../../../../improper-integral.md) is

$$
\int_1^b x^\alpha\,dx=
\begin{cases}
\displaystyle\frac{b^{\alpha+1}-1}{\alpha+1},&\alpha\ne-1,\\[4pt]
\log b,&\alpha=-1.
\end{cases}
$$

This has a finite limit exactly when $\alpha<-1$. If $\alpha\geq0$, the terms $n^\alpha$ do not tend to zero, so the [term test for divergence](../../../../../term-test-for-divergence.md) applies. Thus the full [p-series](../../../../../p-series.md) criterion is

$$
\boxed{\sum_{n\geq1}n^\alpha\text{ converges }\iff\alpha<-1.}
$$

For every $\alpha\geq-1$ its nonnegative [partial sums](../../../../../partial-sum.md) tend to $+\infty$.

## ↑ Ancestors (10)

1. [11D](../11d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
