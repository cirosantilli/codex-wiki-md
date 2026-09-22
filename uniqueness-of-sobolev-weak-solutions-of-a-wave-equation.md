# Uniqueness of Sobolev weak solutions of a wave equation

↑ **Parent:** [Energy method](energy-method.md)

For the [weak energy solution of a variable-coefficient wave equation](weak-energy-solution-of-a-variable-coefficient-wave-equation.md), uniqueness can be proved without using $u_t$ as a spatial $H_0^1$ test function. For a difference with zero data, fix $s$ and test by $v(t)=\int_t^su(r)dr$ for $t<s$, extended by zero afterwards. Put $z(t)=\int_0^tu(r)dr$, so $v(t)=z(s)-z(t)$. [Integration by parts](integration-by-parts.md) in time for the symmetric principal form, and in space for the first-order terms, give

$$
\|u(s)\|_2^2+\theta\|Dz(s)\|_2^2
\leq C\int_0^s\bigl(\|u(t)\|_2^2+\|Dz(t)\|_2^2\bigr)dt+Cs\|Dz(s)\|_2^2.
$$

For short enough intervals the last term is absorbed. The [Gronwall inequality](gronwall-inequality.md) forces $u=0$, and repetition proves uniqueness on the full interval. This antiderivative test is valid at the stated space-time $H^1$ regularity, unlike an unqualified direct energy test by $u_t$.

## ↑ Ancestors (6)

1. [Energy method](energy-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/4/a/ii/solution.md)
