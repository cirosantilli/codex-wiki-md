# Additive composite expansion

↑ **Parent:** [Matched asymptotic expansion](matched-asymptotic-expansion.md)

An [additive composite expansion](additive-composite-expansion.md) combines an [inner expansion](inner-expansion.md) and an [outer expansion](outer-expansion.md) by subtracting their common behavior in the [overlap region](overlap-region.md):

$$
y_{\mathrm{comp}}=y_{\mathrm{out}}+y_{\mathrm{in}}-y_{\mathrm{overlap}}.
$$

The subtraction removes the part counted twice. Near the [boundary layer](boundary-layer.md), the [outer expansion](outer-expansion.md) cancels the overlap contribution; away from the [boundary layer](boundary-layer.md), the [inner expansion](inner-expansion.md) cancels it. An error estimate is needed to establish accuracy across the whole domain.[§4.3.5, p. 58: uniform solution and overlap subtraction](asymptotic-analysis-and-singular-perturbation-theory-by-john-k-hunter.md)

For the [singular perturbation](singular-perturbation-split.md) problem $\epsilon y''+y'=0$, $y(0)=0$, $y(1)=1$, the [outer solution](outer-expansion.md) is one, the leading [inner expansion](inner-expansion.md) is $1-e^{-x/\epsilon}$, and their overlap is one. Thus $y_{\mathrm{comp}}=1-e^{-x/\epsilon}$. With $q=e^{-1/\epsilon}$, comparison with the exact normalized solution gives

$$
y_\epsilon(x)-y_{\mathrm{comp}}(x)
=\frac{q(1-e^{-x/\epsilon})}{1-q},\qquad
\sup_{0\leq x\leq1}|y_\epsilon-y_{\mathrm{comp}}|=q.
$$

The [supremum norm](supremum-norm.md) error is therefore exponentially small on the entire interval, even though the [outer solution](outer-expansion.md) alone has error one. This is an error bound for function values; errors in [derivatives](derivative.md) have additional powers of $\epsilon^{-1}$.

The composite satisfies the [differential equation](differential-equation-split.md) exactly but has right [boundary condition](boundary-condition.md) $y_{\mathrm{comp}}(1)=1-q$. Dividing it by $1-q$ restores that [boundary condition](boundary-condition.md) and recovers the exact solution. This example makes both the strength and the limit of matching explicit: it gives a global approximation, while finite-$\epsilon$ normalization can still carry information beyond every algebraic order.

## ↑ Ancestors (8)

1. [Matched asymptotic expansion](matched-asymptotic-expansion.md)
2. [Singular perturbation](singular-perturbation-split.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Additive composite expansion](additive-composite-expansion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-50/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-336/2/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-336/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-336/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-336/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-336/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-336/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-336/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-336/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-336/3/b/solution.md)
