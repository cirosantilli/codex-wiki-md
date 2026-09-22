# Rodrigues formula for Legendre polynomials

↑ **Parent:** [Legendre polynomial](legendre-polynomial.md)

This instance of [Rodrigues' formula](rodrigues-formula.md) constructs the [Legendre polynomial](legendre-polynomial.md) for every nonnegative [integer](integer-split.md) $l$. Put $v=(x^2-1)^l$; then $(x^2-1)v'=2lxv$. Differentiating $l+1$ times by the [Leibniz rule](leibniz-rule.md) gives $(x^2-1)y''+2xy'-l(l+1)y=0$ for $y=v^{(l)}$, which is the [Legendre differential equation](legendre-differential-equation.md) after reversing signs. The leading term of the normalized derivative is $(2l)!x^l/[2^l(l!)^2]$, proving its [polynomial degree](degree-of-a-polynomial.md) is exactly $l$. At $x=1$, the product $(x+1)^l(x-1)^l$ contributes only the term with all $l$ derivatives on the second factor, giving $v^{(l)}(1)=2^ll!$. Thus the normalization is $P_l(1)=1$.

## ↑ Ancestors (10)

1. [Legendre polynomial](legendre-polynomial.md)
2. [Legendre differential equation](legendre-differential-equation.md)
3. [Second-order linear differential equation](second-order-linear-differential-equation.md)
4. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
5. [Ordinary differential equation](ordinary-differential-equation.md)
6. [Differential equation](differential-equation-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-2/20/b/solution.md)
- [Rodrigues' formula](rodrigues-formula.md)
