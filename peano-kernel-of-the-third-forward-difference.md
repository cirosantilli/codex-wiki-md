# Peano kernel of the third forward difference

↑ **Parent:** [Peano kernel](peano-kernel.md)

For $h>0$, the third [forward difference](forward-difference.md) $L_hu=-u(0)+3u(h)-3u(2h)+u(3h)$ annihilates [polynomials](polynomial-split.md) of degree at most two. Its [Peano kernel](peano-kernel.md) is $K_h(t)=\tfrac12[3(h-t)_+^2-3(2h-t)_+^2+(3h-t)_+^2]$ for $0\leq t\leq3h$, extended by zero outside that interval. It is $h^2$ times the [quadratic cardinal B-spline](quadratic-cardinal-b-spline.md) evaluated at $t/h$, is positive on $(0,3h)$, and has [integral](integral-split.md) $h^3$. The [Peano kernel theorem](peano-kernel-theorem.md) therefore represents $L_hu$ as a positive weighted average of the third [derivative](derivative.md): $L_hu=h^3u^{(3)}(\xi)$ for some interior $\xi$ when that [derivative](derivative.md) is continuous. The kernel is the smooth error weight hidden inside a discrete difference.

## ↑ Ancestors (7)

1. [Peano kernel](peano-kernel.md)
2. [Peano kernel theorem](peano-kernel-theorem.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-approximation-of-functions-course-of-the-university-of-oxford/2011/1/b/solution.md)
