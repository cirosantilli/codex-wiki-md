# Frobenius expansion of the Legendre equation at an endpoint

↑ **Parent:** [Legendre differential equation](legendre-differential-equation.md)

For the [Legendre differential equation](legendre-differential-equation.md) $(1-x^2)y''-2xy'+n(n+1)y=0$, put $t=1+x$. The equation becomes $t(2-t)y_{tt}+2(1-t)y_t+n(n+1)y=0$. Its [indicial equation](indicial-equation.md) is $2r^2=0$. The exponent-zero [power series](power-series.md) $\sum a_kt^k$ obeys the displayed [linear recurrence relation](linear-recurrence-relation.md). For a nonnegative integer $n$, it terminates at degree $n$, giving a [Legendre polynomial](legendre-polynomial.md) with $a_0\ne0$. Every analytic solution at the endpoint is proportional to this one, since the recurrence determines all coefficients from $a_0$.

The second independent solution has the local form $P_n(x)\log(1+x)+B(x)$, where $B$ is analytic near $-1$. Indeed, [reduction of order](reduction-of-order.md) gives $P_n(x)\int dx/[(1-x^2)P_n(x)^2]$, whose integrand is $1/[2P_n(-1)^2(1+x)]$ plus an analytic function. Rescale the second solution to obtain the unit coefficient of $P_n\log(1+x)$. Reflection gives the corresponding expansion at $x=1$. This also proves the logarithmic divergence of the independent [Legendre function of the second kind](legendre-function-of-the-second-kind.md) at each endpoint.

## ↑ Ancestors (9)

1. [Legendre differential equation](legendre-differential-equation.md)
2. [Second-order linear differential equation](second-order-linear-differential-equation.md)
3. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
4. [Ordinary differential equation](ordinary-differential-equation.md)
5. [Differential equation](differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-2-course-of-the-university-of-oxford/2023/2/a/ii/solution.md)
