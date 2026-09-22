<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $y$ be a smooth constrained [minimizer](../../../../global-minimizer.md). For any smooth variation $h$ vanishing at the endpoints, use the normalized admissible curve $y_\varepsilon=(y+\varepsilon h)/\sqrt{J[y+\varepsilon h]}$. Since $J[y]=1$, differentiating at zero gives

$$
0=\left.\frac d{d\varepsilon}I[y_\varepsilon]\right|_0=2\int_0^1\left(xy'h'+\frac{k^2}x yh\right)dx-2I[y]\int_0^1xyh\,dx.
$$

In particular this holds for every compactly supported [test function](../../../../test-function.md) $h$ in $(0,1)$. [Integration by parts](../../../../integration-by-parts.md) and the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) give

$$
-(xy')'+\frac{k^2}x y=I[y]xy,
$$

which is the required [Bessel differential equation](../../../../bessel-differential-equation.md) with $\boxed{\lambda=I[y]}$. The lemma used here says that a continuous function whose integral against every compactly supported smooth [test function](../../../../test-function.md) is zero must itself vanish. No multiplier-existence theorem is needed: the explicit normalization produces the variation directly.

The endpoint $0$ causes no divergent energy for these variations: smoothness and $y(0)=h(0)=0$ imply $y,h=O(x)$. Also $J[v]>0$ for every nonzero admissible $v$, and $v/\sqrt{J[v]}$ has unit $J$ and energy $I[v]/J[v]$. Thus minimizing $I$ with $J=1$ is equivalent to minimizing the scale-invariant [Rayleigh quotient](../../../../rayleigh-quotient.md) $I/J$. The zero function is excluded whenever this quotient is written.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
