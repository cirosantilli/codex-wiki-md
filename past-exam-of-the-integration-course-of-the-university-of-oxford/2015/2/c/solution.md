<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every fixed $x>0$, $\log(x+n)/n\to0$, so $f_n(x)\to0$. To exchange the [limit](../../../../limit-of-a-function.md) with the [Lebesgue integral](../../../../lebesgue-integral.md), we need a common integrable bound over the whole half-line.

For $n\geq1$, $x+n\leq n(1+x)$, so

$$
0\leq\frac{\log(x+n)}n
\leq\frac{\log n}{n}+\frac{\log(1+x)}n
\leq1+\log(1+x).
$$

Together with $|\sin x|\leq\min(x,1)$, this gives

$$
|f_n(x)|\leq G(x):=\bigl(1+\log(1+x)\bigr)\frac{\min(x,1)}{x^q}.
$$

For $0<x\leq1$, $\log(1+x)\leq x\leq1$, hence $G(x)\leq2x^{1-q}$, which is integrable because $q<2$. For $x\geq1$,

$$
G(x)\leq\frac{1+\log2+\log x}{x^q}.
$$

Both terms are integrable because $q>1$:

$$
\int_1^\infty x^{-q}\,dx=\frac1{q-1},\qquad
\int_1^\infty\frac{\log x}{x^q}\,dx=\frac1{(q-1)^2}.
$$

The second equality follows from [integration by parts](../../../../integration-by-parts.md), or the [substitution](../../../../substitution-algebra.md) $x=e^t$. Consequently $G$ is a [Lebesgue integrable function](../../../../lebesgue-integrable-function.md), and every $f_n$ is [Lebesgue integrable](../../../../lebesgue-integrable-function.md).

The [dominated convergence theorem](../../../../dominated-convergence-theorem.md) states that [almost everywhere](../../../../almost-everywhere.md) convergence of [measurable functions](../../../../measurable-function.md) under one integrable absolute-value bound implies [L1 convergence](../../../../convergence-in-l1.md), and in particular convergence of their [integrals](../../../../integral-split.md). Here the pointwise [limit](../../../../limit-of-a-function.md) is zero and the dominator is $G$, so

$$
\boxed{\lim_{n\to\infty}\int_0^\infty f_n(x)\,dx=0.}
$$

In fact we obtain the stronger conclusion $\|f_n\|_1\to0$. A quantitative version follows by retaining the factors $1/n$ in the bound:

$$
\|f_n\|_1\leq\frac{A\log n+B}{n},
\quad
A=\int_0^\infty\frac{|\sin x|}{x^q}\,dx,
\quad
B=\int_0^\infty\frac{\log(1+x)|\sin x|}{x^q}\,dx.
$$

The preceding endpoint estimates show $A,B<\infty$, so the [L1 norm](../../../../l1-norm.md) is $O(\log n/n)$ as $n\to\infty$, with $O$ denoting [Big O notation](../../../../big-o-notation.md). This is [logarithmic reweighting under dominated convergence](../../../../logarithmic-reweighting-under-dominated-convergence.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
