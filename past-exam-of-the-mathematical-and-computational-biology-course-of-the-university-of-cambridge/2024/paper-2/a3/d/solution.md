<h1 id="a3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $x=1.5+e^y$. Every finite unconstrained value of $y$ then gives an allowed point with $x>1.5$:


```
def transformed(y):
    return f(1.5 + np.exp(y[0]))


result = opt.minimize(transformed, x0=[0.0])
x_interior = 1.5 + np.exp(result.x[0])
x_best = min([1.5, x_interior], key=f)
print(x_best, f(x_best))
```
Explicitly checking $x=1.5$ covers the boundary omitted by the exponential transformation. The minimum is **$x\simeq2.164817$, $f(x)\simeq0.614056$**, whereas $f(1.5)\simeq1.59810$.

[Constraint reparameterization](../../../../../constraint-reparameterization.md) enforces feasibility but does not remove nonconvexity. In this example, $f\geq1$ up to the next negative-sine lobe, the [derivative](../../../../../derivative.md) has one minimum in that lobe, and for $x\geq4\pi/5$ the envelope gives $f(x)\geq1-e^{-16\pi^2/125}\simeq0.7173$. Thus later oscillations cannot improve on the displayed constrained minimum.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [A3](../../a3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
