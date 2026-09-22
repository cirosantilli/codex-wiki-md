<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Prove the [natural-number fold fusion law](../../../../../natural-number-fold-fusion-law.md) pointwise. At `Zero`,

```
f (foldNat g a Zero) = f a = b = foldNat h b Zero
```

Assuming the equation at `m`, the `Succ m` calculation is:

```
f (foldNat g a (Succ m))
  = f (g (foldNat g a m))
  = h (f (foldNat g a m))
  = h (foldNat h b m)
  = foldNat h b (Succ m)
```

The compatibility premise `f . g = h . f` justifies the middle rewrite. This proves the theorem for finite total constructor values by [structural induction](../../../../../structural-induction.md).

For the full lazy [Haskell](../../../../../haskell.md) interpretation, also handle the [bottom value](../../../../../bottom-value.md): `foldNat g a` is strict in its outer `Natural` constructor, so its value on bottom is bottom; the assumed [strict function](../../../../../strict-function.md) property of `f` makes the left side bottom too. The same zero/successor induction now covers finite partial constructor chains. Pure definable functions preserve the limits of these information approximations, extending equality to infinite `Succ` chains. This explains the strictness premise; finite total induction alone would not use it.[§3.1: bottom values; §6.2: strict evaluation](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
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
