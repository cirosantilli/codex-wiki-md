# Bilinear interpolation

↑ **Parent:** [Interpolation](interpolation-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bilinear_interpolation)

On a rectangle, [bilinear interpolation](bilinear-interpolation.md) is linear in each coordinate separately and matches the four corner values. With normalized coordinates $s,t\in[0,1]$, it is $(1-s)(1-t)u_{00}+s(1-t)u_{10}+(1-s)tu_{01}+stu_{11}$. A [multigrid method](multigrid-method-split.md) can use it to prolong a coarse correction to finer-grid nodes. It is not generally an affine function of the pair $(s,t)$, since it can contain a mixed $st$ term.

## ↑ Ancestors (6)

1. [Interpolation](interpolation-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bilinear interpolation](bilinear-interpolation.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/a/3/a/solution.md)
