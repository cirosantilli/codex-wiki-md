# Logarithmic quadratic parameter integral

↑ **Parent:** [Differentiation under the integral sign](differentiation-under-the-integral-sign.md)

For every real parameter $a$,

$$
\boxed{F(a)=\int_0^\infty\frac{a\ln(a^2+x^2)}{1+x^2}\,dx=\pi a\ln(1+|a|),}
$$

where $F(0)=0$. For $a>0$, [differentiation under the integral sign](differentiation-under-the-integral-sign.md) and a [partial fraction decomposition](partial-fraction-decomposition.md) give

$$
F'(a)-F(a)/a=2a^2\int_0^\infty\frac{dx}{(x^2+a^2)(1+x^2)}=\frac{\pi a}{1+a}.
$$

Solving this [first-order linear differential equation](first-order-linear-differential-equation.md) yields $F(a)=a[\pi\ln(1+a)+C]$. To fix the constant, [dominated convergence](dominated-convergence-theorem.md) gives $\lim_{a\to0^+}F(a)/a=\int_0^\infty\ln(x^2)/(1+x^2)dx=0$; the last absolutely convergent [integral](integral-split.md) changes sign under $x=1/t$. Thus $C=0$. Oddness in $a$ supplies the result for negative parameters. The initial value $F(0)=0$ alone does not determine $C$, since every solution $a[\pi\ln(1+a)+C]$ tends to zero as $a\to0^+$.

## ↑ Ancestors (5)

1. [Differentiation under the integral sign](differentiation-under-the-integral-sign.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/20/b/solution.md)
