# Klee-Minty cube

↑ **Parent:** [Simplex method](simplex-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Klee–Minty_cube)

For $0<\varepsilon<1/2$, these inequalities define a deformed [cube](cube.md) with $2^n$ [vertices of a polytope](vertex-of-a-polytope.md). Choose either the lower or upper bound recursively at each coordinate to obtain a [vertex of a polytope](vertex-of-a-polytope.md); changing one choice gives an adjacent [vertex of a polytope](vertex-of-a-polytope.md). When maximizing $x_n$, smallest-index improving-facet pivoting visits all $2^n$ [vertices of a polytope](vertex-of-a-polytope.md): first traverse the lower last-coordinate face, then move to the upper face and traverse the preceding path in reverse. Thus this geometric version of the [Bland pivoting rule](bland-pivoting-rule.md) can require $2^n-1$ pivots. Rescaling the coordinate $x_i$ to $y_i=\varepsilon^{2(n-i)}x_i$ makes the positive rate per unit freed coordinate equal to $\varepsilon^{-(n-i)}$; [Dantzig pivot rule](dantzig-pivot-rule.md) then selects the same exponential path. Euclidean edge-length pricing is a different rule.

## ↑ Ancestors (6)

1. [Simplex method](simplex-method.md)
2. [Linear programming](linear-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Dantzig pivot rule](dantzig-pivot-rule.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38/2/solution.md)
