<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For exact ordered numbers, first discard multipliers equal to one and reject those below one:

```
hamming' :: (Ord a, Num a) => [a] -> [a]
hamming' as
  | any (<1) as = error "multipliers below one violate the ordered contract"
  | otherwise  = hs
  where
    bs = filter (>1) as
    hs = 1 : case bs of
               [] -> []
               _  -> foldr1 merge [map (a*) hs | a <- bs]
```

The [type signature](../../../../../type-signature.md) has exactly the numeric and ordering constraints used by the definition. For a finite nonempty collection of multipliers greater than one, this is the same [sorted multiplicative closure stream](../../../../../sorted-multiplicative-closure-stream.md) construction as before, merging one scaled copy per multiplier. It is infinite and strictly increasing; local finiteness below any bound and the smaller-predecessor argument prove completeness and [productivity](../../../../../stream-productivity.md). In particular, `[2,3,5]` reproduces `hamming`.

**The literal contract for arbitrary positive multipliers is impossible.** A multiplier strictly between zero and one would require a value smaller than the initial one; an empty list or the list `[1]` generates only one value. The definition returns the finite closure `[1]` in those degenerate cases. A multiplier equal to one adds no mathematical values and would introduce an unnecessary circular merge demand if left in the feedback streams. The order and growth proof assumes exact arithmetic with the usual laws; the broad numeric type alone cannot prevent floating-point rounding or bounded overflow.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
