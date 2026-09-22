# Concave Legendre dual

↑ **Parent:** [Convex conjugate](convex-conjugate.md)

For a differentiable strictly [concave function](concave-function.md) $f$ whose derivative is a bijection of $\mathbb R$, define

$$
g(z)=\inf_{s\in\mathbb R}\{zs-f(s)\}=zh(z)-f(h(z)),\qquad h=(f')^{-1}.
$$

The unique minimizing point is $h(z)$, and $g'=h$ follows by comparing minimizers at adjacent arguments, even when $h$ is not differentiable. This dual is concave and equals $-(-f)^*(-z)$ in terms of the [convex conjugate](convex-conjugate.md). If $f''<0$, then $g''=1/f''(h)$. For $f(s)=cs-s^2/2$, $g(z)=-(z-c)^2/2$.

**Table of contents**

- [Lower conjugate](lower-conjugate.md)
  - [Concave biconjugate](concave-biconjugate.md)
- [Inverse-flux quadratic bounds](inverse-flux-quadratic-bounds.md)

## ↑ Ancestors (6)

1. [Convex conjugate](convex-conjugate.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Inverse-flux quadratic bounds](inverse-flux-quadratic-bounds.md)
- [Maximum representation for a concave conservation law](maximum-representation-for-a-concave-conservation-law.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/1/3/e/solution.md)
- [Wealth-variable Legendre dual](wealth-variable-legendre-dual.md)
