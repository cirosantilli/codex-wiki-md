# Signed area under a graph

↑ **Parent:** [Integral](integral.md)

For $a<b$ and a [real-valued function](real-valued-function.md) $f$ with a finite [Riemann integral](riemann-integral.md) or [Lebesgue integral](lebesgue-integral.md) on $[a,b]$, the [signed area under a graph](signed-area-under-a-graph.md) is its [definite integral](definite-integral.md): geometric [area](surface-area.md) above the horizontal axis contributes positively, and geometric [area](surface-area.md) below it contributes negatively. If these two nonnegative [areas](surface-area.md) are $A_+$ and $A_-$, then

$$
\int_a^b f(x)\,dx=A_+-A_-,\qquad
\int_a^b |f(x)|\,dx=A_++A_-.
$$

The second expression is the [total geometric area under a graph](total-geometric-area-under-a-graph.md). Taking the [absolute value](absolute-value.md) of the first expression does not usually give the second: cancellation has already removed information about how much [area](surface-area.md) lies on each side.[5.2 The Definite Integral](calculus-volume-1-by-gilbert-strang-and-others/5-2-the-definite-integral.md)

For an exact example, take the [polynomial function](polynomial-function.md) $f(x)=x^2-1$ on $[-2,2]$. Its [polynomial roots](root-of-a-polynomial.md) are $-1$ and $1$: it is negative between them and positive on the two outer [intervals](interval-mathematics.md). An [antiderivative](antiderivative.md) is $F(x)=x^3/3-x$, so the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) gives

$$
\int_{-2}^{-1}(x^2-1)\,dx=\frac43,\qquad
\int_{-1}^{1}(x^2-1)\,dx=-\frac43,\qquad
\int_{1}^{2}(x^2-1)\,dx=\frac43.
$$

Thus $A_+=8/3$ and $A_-=4/3$. The [signed area under a graph](signed-area-under-a-graph.md) is $4/3$, whereas the [total geometric area under a graph](total-geometric-area-under-a-graph.md) is $4$. To compute the latter with [antiderivatives](antiderivative.md), split at each sign-changing [polynomial root](root-of-a-polynomial.md) and reverse the sign of the negative contribution.

<a id="signed-polynomial-area-and-absolute-area"></a>
![](signed-polynomial-area-and-absolute-area.png)

**[Figure 6](#signed-polynomial-area-and-absolute-area). The polynomial x squared minus one has signed integral 4/3 and total geometric area 4 on the interval from minus two to two**.

Cancellation is useful information when the [integrand](integrand.md) represents a signed contribution. For the [polynomial function](polynomial-function.md) $f(x)=x$ on $[-1,1]$, the two triangular [areas](surface-area.md) give $\int_{-1}^1x\,dx=0$, although $\int_{-1}^1|x|\,dx=1$. Zero [net signed area](signed-area-under-a-graph.md) therefore means balanced positive and negative contributions, rather than an empty region.

The short algebraic justification uses the [positive part](positive-part-of-a-real-valued-function.md) $f_+=\max(f,0)$ and [negative part](negative-part-of-a-real-valued-function.md) $f_-=\max(-f,0)$: $f=f_+-f_-$ and $|f|=f_++f_-$. Their [integrals](integral.md) give $A_+$ and $A_-$, and [linearity of integration](linearity-of-integration.md) gives the difference and sum formulas. For [Lebesgue integration](lebesgue-integration.md), require both contributions to be finite to avoid the undefined subtraction $\infty-\infty$.[Definitions 120–121 and Proposition 122](18-102-introduction-to-functional-analysis-spring-2021-lecture-notes-by-andrew-lin/lecture-12-lebesgue-integrable-functions-the-lebesgue-integral-and-the-dominated-convergence-theorem.md)

**Table of contents**

- [Total geometric area under a graph](total-geometric-area-under-a-graph.md)

## ↑ Ancestors (7)

1. [Integral](integral.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cauchy principal value](cauchy-principal-value.md)
- [Integral](integral.md)
- [Signed area under a graph](signed-area-under-a-graph.md)
