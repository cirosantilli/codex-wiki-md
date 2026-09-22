# Function-value resolution near a nondegenerate minimum

↑ **Parent:** [Round-off error](round-off-error.md)

Near a smooth [local minimum](local-minimum.md) $x_*$ with $f'(x_*)=0$ and $f''(x_*)>0$, [Taylor's theorem](taylor-s-theorem.md) gives

$$
f(x_*+h)-f(x_*)=\tfrac12 f''(x_*)h^2+o(h^2).
$$

If evaluated [function](function-split.md) values have absolute uncertainty of order $\delta f$, differences on that scale cannot reliably identify smaller displacements than order $\sqrt{\delta f/f''(x_*)}$. In ordinary [floating-point arithmetic](floating-point-arithmetic-split.md), when $f(x_*)\ne0$ and evaluations have relative error of order $\epsilon$, this becomes

$$
|h|\sim\sqrt{\epsilon\,\frac{|f(x_*)|}{f''(x_*)}}.
$$

For unit-scale values and curvature, this is the square root of [machine epsilon](machine-epsilon.md), rather than machine epsilon itself. It explains why a [derivative](derivative.md)-free [golden-section search](golden-section-search.md) can lose reliable comparisons while candidate positions remain representably different.[Caveats: loss of the quadratic term when added to a nonzero minimum value](one-dimensional-minimization-in-the-gnu-scientific-library-manual.md)

This is a precision limit of the evaluated values, not an invariant property of the minimizer. Accurately subtracting a known constant, obtaining values at higher precision, or locating a zero of an accurately evaluated [derivative](derivative.md) can change the attainable position accuracy. A zero minimum with relative error controlled on its small values also needs separate analysis.

## ↑ Ancestors (6)

1. [Round-off error](round-off-error.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/4/e/solution.md)
