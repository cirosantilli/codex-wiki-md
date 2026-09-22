# Finite volume method

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_volume_method)

A finite volume method evolves cell integrals or cell averages by differences of shared interface [numerical fluxes](numerical-flux.md). For a [scalar conservation law](scalar-conservation-law.md), $U_j^{n+1}=U_j^n-(k/d)(F_{j+1/2}-F_{j-1/2})$. Sharing the same flux between neighboring cells makes conservation follow by telescoping.

**Table of contents**

- [Monotone conservative scheme](monotone-conservative-scheme.md)
  - [Total variation diminishing scheme](total-variation-diminishing-scheme.md)
  - [L1 contraction of a monotone conservative scheme](l1-contraction-of-a-monotone-conservative-scheme.md)
  - [Engquist-Osher method](engquist-osher-method.md)
    - [CFL necessity for explicit Engquist-Osher stability](cfl-necessity-for-explicit-engquist-osher-stability.md)
    - [Engquist-Osher flux](engquist-osher-flux.md)
      - [Sonic-point splitting of a convex Engquist-Osher flux](sonic-point-splitting-of-a-convex-engquist-osher-flux.md)
- [Numerical flux](numerical-flux.md)
  - [Godunov numerical flux](godunov-numerical-flux.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Engquist-Osher method](engquist-osher-method.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/6/solution.md)
