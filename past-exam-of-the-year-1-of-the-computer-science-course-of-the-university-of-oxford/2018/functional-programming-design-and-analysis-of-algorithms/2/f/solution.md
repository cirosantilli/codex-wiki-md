<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The coefficient index supplies the multiplier for a [formal derivative](../../../../../formal-derivative.md) and the divisor for a zero-constant [formal integral](../../../../../formal-integral.md):

```
deriv :: Num a => [a] -> [a]
deriv as = zipWith (*) (map fromInteger [1..]) (tail as)

integral :: Fractional a => [a] -> [a]
integral as = 0 : zipWith (/) as (map fromInteger [1..])
```

Using `fromInteger` makes the index stream unbounded before conversion to the coefficient type. The [formal derivative](../../../../../formal-derivative.md) drops the original constant coefficient; the [formal integral](../../../../../formal-integral.md) prepends its chosen zero constant. With exact `Rational` coefficients these are exact algebraic operations. Analytic [convergence](../../../../../convergence.md) is unnecessary for operations on [formal power series](../../../../../formal-power-series.md) over a characteristic-zero field.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
