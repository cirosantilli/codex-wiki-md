# Meromorphic continuation of a Mellin transform from an asymptotic expansion

↑ **Parent:** [Mellin transform](mellin-transform.md)

Suppose $f$ decays faster than every power at infinity and, near zero, $f(y)=\sum_{j=1}^r c_jy^{\sigma_j}+O(y^{\sigma_{r+1}})$ for every $r$, with $\sigma_j$ strictly increasing and tending to infinity. Subtracting finitely many terms in the integral over $(0,1)$ gives

$$
\mathcal Mf(s)=\int_1^\infty f(y)y^{s-1}\,dy+\sum_{j=1}^r\frac{c_j}{s+\sigma_j}+\int_0^1\left(f(y)-\sum_{j=1}^r c_jy^{\sigma_j}\right)y^{s-1}\,dy.
$$

The last integral is [holomorphic](complex-differentiability-at-a-point.md) on $\operatorname{Re}s>-\sigma_{r+1}$. These expressions continue the [Mellin transform](mellin-transform.md) meromorphically to the whole plane, with simple poles precisely at $-\sigma_j$ for nonzero $c_j$.

**Table of contents**

- [Accumulating asymptotic exponents obstruct Mellin continuation](accumulating-asymptotic-exponents-obstruct-mellin-continuation.md)

## ↑ Ancestors (6)

1. [Mellin transform](mellin-transform.md)
2. [Integral transform](integral-transform.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bernoulli formula for zeta values at nonpositive integers](bernoulli-formula-for-zeta-values-at-nonpositive-integers.md)
- [Mellin continuation of a nonprincipal Dirichlet L-function](mellin-continuation-of-a-nonprincipal-dirichlet-l-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-137/1/solution.md)
