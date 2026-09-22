<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $a<b$, the one-panel [trapezoidal rule](../../../../trapezoidal-rule.md) is

$$
\boxed{\int_a^b f(x)\,dx\ \approx\ T(f):=\frac{b-a}{2}\bigl(f(a)+f(b)\bigr).}
$$

It integrates the [linear interpolation](../../../../linear-interpolation.md) between the two endpoint samples. Indeed the [affine function](../../../../affine-function.md)

$$
\ell(x)=\frac{b-x}{b-a}f(a)+\frac{x-a}{b-a}f(b)
$$

has [definite integral](../../../../definite-integral.md) $T(f)$. The two [quadrature nodes](../../../../quadrature-node.md) are $a,b$ and both [quadrature weights](../../../../quadrature-weight.md) are $(b-a)/2$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
