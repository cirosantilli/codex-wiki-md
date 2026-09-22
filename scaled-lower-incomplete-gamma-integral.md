# Scaled lower incomplete gamma integral

↑ **Parent:** [Incomplete gamma function](incomplete-gamma-function.md)

For $a>0$, this [integral](integral-split.md) is an [entire function](entire-function.md) of $x$: the [exponential series](exponential-series.md) converges uniformly on bounded subsets after multiplication by the [integrable](integrability.md) bound $e^{|x|}u^{a-1}$. Thus

$$
F_a(x)=\sum_{m=0}^{\infty}\frac{(-x)^m}{m!(a+m)},\qquad F_a^{(m)}(0)=\frac{(-1)^m}{a+m}.
$$

For positive real $x$, a [change of variables](change-of-variables-formula.md) gives $F_a(x)=x^{-a}\gamma(a,x)$, where here $\gamma(a,x)=\int_0^xe^{-t}t^{a-1}dt$ denotes the lower [incomplete gamma function](incomplete-gamma-function.md). The singular-looking factor $x^{-a}$ is removed by the integral over $[0,1]$. Applying [integration by parts](integration-by-parts.md) to the [derivative](derivative.md) of $u^ae^{-xu}$ gives $xF_a'+aF_a=e^{-x}$; differentiating and eliminating $e^{-x}$ proves $xF_a''+(a+1+x)F_a'+aF_a=0$.

## ↑ Ancestors (5)

1. [Incomplete gamma function](incomplete-gamma-function.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/section-b/10/a/solution.md)
