<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Both rules use a uniform partition with $\Delta x=(b-a)/n$. An original implementation in pseudocode is:

```
function trapezoid(f, a, b, n):
    dx = (b-a)/n
    total = (f(a)+f(b))/2
    for j in 1,...,n-1:
        total += f(a+j*dx)
    return dx*total

function midpoint(f, a, b, n):
    dx = (b-a)/n
    total = 0
    for j in 0,...,n-1:
        total += f(a+(j+1/2)*dx)
    return dx*total
```

The [trapezoidal rule](../../../../../trapezoidal-rule.md) gives each endpoint half weight; the [composite midpoint rule](../../../../../composite-midpoint-quadrature-rule.md) uses one interior point per subinterval. Both converge for a continuous [integrand](../../../../../integrand.md) on the closed interval.

**The second equality in the printed trapezoidal hint is missing a factor $1/2$.** The average of the left and right rectangle sums is required. For $f=1$, the uncorrected equality would return $2(b-a)$ instead of $b-a$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
