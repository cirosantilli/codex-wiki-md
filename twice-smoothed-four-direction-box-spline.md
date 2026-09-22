# Twice-smoothed four-direction box spline

↑ **Parent:** [Box spline](box-spline.md)

Take two copies of each direction $(1,0),(0,1),(1,1),(1,-1)$. The resulting [box spline](box-spline.md) has total polynomial degree six and $C^4$ continuity: there are eight directions and a rank-deficient remaining set has at most two, so the removal number is six. With a centred origin its support is the [zonotope](zonotope.md)

$$
\{|x|\leq3,\ |y|\leq3,\ |x|+|y|\leq4\}.
$$

Its centred binary symbol is

$$
\frac{(1+z)^2(1+w)^2(1+zw)^2(1+z/w)^2}{64z^3w}.
$$

This symbol factors as $A(z,w)A(zw,z/w)$ with $A=(2+z+z^{-1})(2+w+w^{-1})/8$, giving an efficient [quincunx subdivision](quincunx-subdivision.md) implementation. The [box spline](box-spline.md) criterion is also described in the primary research paper [4–8 Subdivision](https://cims.nyu.edu/gcl/papers/velho20014s.pdf) by Velho and Zorin.

## ↑ Ancestors (8)

1. [Box spline](box-spline.md)
2. [Spline approximation](spline-approximation.md)
3. [Spline (mathematics)](spline-mathematics.md)
4. [Uniform approximation](uniform-approximation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/5/d/solution.md)
