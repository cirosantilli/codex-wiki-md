# Leibniz integral rule

↑ **Parent:** [Differentiation under the integral sign](differentiation-under-the-integral-sign.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Leibniz_integral_rule)

For differentiable endpoints $a,b$ and a [function](function-split.md) $f$ with suitable continuous [partial derivative](partial-derivative.md) in the parameter, the moving-endpoint rule is

$$
\boxed{\frac d{dx}\int_{a(x)}^{b(x)}f(x,t)\,dt=f(x,b(x))b'(x)-f(x,a(x))a'(x)+\int_{a(x)}^{b(x)}f_x(x,t)\,dt.}
$$

To prove it locally, put $H(x,u)=\int_c^u f(x,t)\,dt$ for a fixed reference endpoint $c$. The original [integral](integral-split.md) is $H(x,b(x))-H(x,a(x))$. Apply the [chain rule](chain-rule.md), use the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) for $H_u=f$, and use [differentiation under the integral sign](differentiation-under-the-integral-sign.md) for $H_x$. The two boundary terms account for the moving endpoints, while the remaining [integral](integral-split.md) accounts for variation of the integrand with the parameter. For [improper integrals](improper-integral.md), convergence and a suitable domination condition must be verified before interchanging the [derivative](derivative.md) and [integral](integral-split.md).

## ↑ Ancestors (5)

1. [Differentiation under the integral sign](differentiation-under-the-integral-sign.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Derivative of an Abel integral](derivative-of-an-abel-integral.md)
- [Differentiating a principal-value integral across a fixed simple pole](differentiating-a-principal-value-integral-across-a-fixed-simple-pole.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-2/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/section-b/10/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/19/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/20/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/20/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/20/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/20/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/20/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/20/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/20/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/8/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/5/solution.md)
