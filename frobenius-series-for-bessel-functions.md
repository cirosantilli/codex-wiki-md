# Frobenius series for Bessel functions

↑ **Parent:** [Bessel differential equation](bessel-differential-equation.md)

For the [Bessel differential equation](bessel-differential-equation.md) $x^2y''+xy'+(x^2-\nu^2)y=0$, substitute $y=x^s\sum_{n\geq0}a_nx^n$. The [indicial equation](indicial-equation.md) is $s^2-\nu^2=0$, and coefficients obey $[(n+s)^2-\nu^2]a_n=-a_{n-2}$. For $s=\nu\geq0$, $a_1=0$ and all odd coefficients vanish. Iteration gives $a_{2m}=(-1)^ma_0\Gamma(\nu+1)/[4^mm!\Gamma(m+\nu+1)]$. Choosing $a_0=1/[2^\nu\Gamma(\nu+1)]$ gives the [Bessel function of the first kind](bessel-function-of-the-first-kind.md) $J_\nu$.

For noninteger $\nu$, choosing the even-power series with $s=-\nu$ replaces $m+\nu$ by $m-\nu$ and yields $J_{-\nu}$ with its standard normalization. These solutions are independent. For integer $\nu\geq0$, the first solution has coefficients $(-1)^m/[2^{2m+\nu}m!(m+\nu)!]$ and defines an entire function: the term ratio tends to zero at every finite complex argument. For noninteger order, the even analytic series converges everywhere, while the prefactor $x^{\pm\nu}$ requires a branch off the positive real axis.

## ↑ Ancestors (6)

1. [Bessel differential equation](bessel-differential-equation.md)
2. [Bessel function](bessel-function-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-1/6/solution.md)
