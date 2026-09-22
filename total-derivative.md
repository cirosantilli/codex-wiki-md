# Total derivative

↑ **Parent:** [Derivative](derivative.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Total_derivative)

A [total derivative](total-derivative.md) accounts for every dependence of a quantity on the variable of [differentiation](differentiation.md). For a [differentiable function](differentiable-function.md) $F(t,x_1,\ldots,x_n)$ evaluated along [differentiable](differentiable-function.md) coordinate [functions](function-split.md) $x_i(t)$, the [multivariable chain rule](multivariable-chain-rule.md) gives

$$
\frac{d}{dt}F(t,x_1(t),\ldots,x_n(t))
=\frac{\partial F}{\partial t}+\sum_{i=1}^n\frac{\partial F}{\partial x_i}\frac{dx_i}{dt}.
$$

All the [partial derivatives](partial-derivative.md) on the right are evaluated at $(t,x_1(t),\ldots,x_n(t))$. The first term captures explicit dependence on $t$; the remaining terms capture changes transmitted through the coordinates.

For example, take $F(t,x)=tx^2$ and $x(t)=t$. The [partial derivative](partial-derivative.md) with respect to $t$, holding $x$ fixed, is $x^2$, whose value on the path is $t^2$. The [total derivative](total-derivative.md) is instead

$$
\frac d{dt}F(t,t)=\frac d{dt}t^3=3t^2
=\underbrace{t^2}_{\partial_t F}+\underbrace{2t^2}_{\partial_x F\,x'}.
$$

At $t=2$, the [partial derivative](partial-derivative.md) is $4$ and the [total derivative](total-derivative.md) is $12$. The difference is the contribution from changing $x$.

If the composite [function](function-split.md) is [continuously differentiable](continuously-differentiable-function.md) on $[a,b]$, the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) gives

$$
\int_a^b\frac{d}{dt}F(t,x(t))\,dt=F(b,x(b))-F(a,x(a)).
$$

This is the sense in which an integrated [total derivative](total-derivative.md) contributes endpoint terms. The endpoint statement concerns the whole composite [function](function-split.md) along the path. [OpenStax, Calculus Volume 3: the chain rule with dependent variables](https://openstax.org/books/calculus-volume-3/pages/4-5-the-chain-rule).

## ↑ Ancestors (7)

1. [Derivative](derivative.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Chiral proof of rigid worldsheet supersymmetry](chiral-proof-of-rigid-worldsheet-supersymmetry.md)
- [Covector](covector.md)
- [Neutral Coulomb pair in a uniform magnetic field](neutral-coulomb-pair-in-a-uniform-magnetic-field.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-48/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-48/2/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/8e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-306/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-337/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-337/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-337/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-337/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/9/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/9/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/9/e/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2013/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2018/3/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2019/3/c/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2022/1/c/solution.md)
- [Total derivative](total-derivative.md)
- [Total time derivatives preserve fixed-endpoint Euler-Lagrange equations](total-time-derivatives-preserve-fixed-endpoint-euler-lagrange-equations.md)
