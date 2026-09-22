# Logarithmic sine integral

↑ **Parent:** [Differentiation under the integral sign](differentiation-under-the-integral-sign.md)

For every real $a$, define $I(a)=\int_0^1\sin(a\log x)/\log x\,dx$. The apparent endpoint singularity at $x=1$ is removable, with limit $a$, and the bound $|\sin(a\log x)/\log x|\leq|a|$ ensures integrability. [Differentiation under the integral sign](differentiation-under-the-integral-sign.md) is justified by the integrable bound $|\cos(a\log x)|\leq1$ on the parameter derivative. Thus

$$
I'(a)=\int_0^1\cos(a\log x)\,dx
=\int_0^\infty e^{-t}\cos(at)\,dt=\frac1{1+a^2},
$$

where $x=e^{-t}$ and the last integral is a [Laplace transform](laplace-transform.md). Since $I(0)=0$, integrating with respect to $a$ gives $I(a)=\arctan a$. This obtains an integral with a logarithmic denominator by differentiating away that denominator, then restoring the parameter dependence with one elementary antiderivative.

## ↑ Ancestors (5)

1. [Differentiation under the integral sign](differentiation-under-the-integral-sign.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/20/c/solution.md)
