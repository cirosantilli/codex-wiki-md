# Rational lower bound for the natural logarithm

↑ **Parent:** [Logarithm inequality](logarithm-inequality.md)

For $t>0$, the [natural logarithm](natural-logarithm.md) satisfies

$$
\boxed{\ln(1+t)>\frac{2t}{2+t}.}
$$

To prove it, put $h(t)=\ln(1+t)-2t/(2+t)$. Then $h(0)=0$ and the [derivative](derivative.md) is $h'(t)=t^2/[(1+t)(2+t)^2]>0$. More precisely,

$$
h(t)=\int_0^t\frac{s^2}{(1+s)(2+s)^2}\,ds.
$$

This positive [integral](integral-split.md) controls errors in symmetric approximations to the [logarithm](logarithm.md). After writing $x=1+t$, the bound is $\ln x>2(x-1)/(x+1)$ for $x>1$; the inequality reverses for $0<x<1$ by replacing $x$ with $1/x$.

## ↑ Ancestors (9)

1. [Logarithm inequality](logarithm-inequality.md)
2. [Logarithm](logarithm.md)
3. [Exponential function](exponential-function.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Convergence of the Stirling sequence](convergence-of-the-stirling-sequence.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/19/d/solution.md)
