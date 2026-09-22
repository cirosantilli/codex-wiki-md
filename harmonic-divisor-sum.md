# Harmonic divisor sum

↑ **Parent:** [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)

Write $B(t)=\sum_{n\leq t}\tau(n)/n$ and $r=\lfloor\sqrt t\rfloor$. The weighted [Dirichlet hyperbola method](dirichlet-hyperbola-method.md) gives

$$
B(t)=2\sum_{a\leq r}\frac{H_{\lfloor t/a\rfloor}}a-H_r^2
=\tfrac12\log^2t+2\gamma\log t+c+O\left(\frac{\log(2t)}{\sqrt t}\right).
$$

Indeed, use $H_{\lfloor u\rfloor}=\log u+\gamma+O(1/u)$ and $\sum_{a\leq r}(\log a)/a=\tfrac12\log^2r+c\prime+O(\log(2r)/r)$. The latter follows by comparing each summand with the integral on its unit interval: the derivative of $(\log t)/t$ has an integrable tail. Since $r=\sqrt t+O(1)$, substitution yields the expansion. Here $H_n$ is the [harmonic number](harmonic-number.md) and $\gamma$ the [Euler--Mascheroni constant](euler-s-constant.md).

## ↑ Ancestors (7)

1. [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)
2. [Dirichlet convolution](dirichlet-convolution.md)
3. [Arithmetic function](arithmetic-function.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Möbius harmonic logarithmic moments](mobius-harmonic-logarithmic-moments.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/5/b/solution.md)
