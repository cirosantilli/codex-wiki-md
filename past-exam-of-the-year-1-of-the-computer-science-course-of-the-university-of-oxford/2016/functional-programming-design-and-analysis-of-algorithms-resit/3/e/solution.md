<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Compose the three parsing stages using the supplied [fold](../../../../../fold.md), and accept only when no suffix remains:
```
eval :: String -> Maybe Int
eval input = foldMaybe first Nothing (parseInt input)
  where
    first (a,rest) = foldMaybe (second a) Nothing (parseOp rest)
    second a (op,rest) = foldMaybe (finish a op) Nothing (parseInt rest)
    finish a op (b,rest)
      | null rest = Just (apply op a b)
      | otherwise = Nothing
    apply '+' a b = a+b
    apply '-' a b = a-b
    apply '*' a b = a*b
    apply '/' a b = a `div` b
    apply _ _ _ = error "unreachable: parseOp rejected this operator"
```
Every failed intermediate [parser](../../../../../parser.md) is converted to `Nothing` by `foldMaybe`. Checking `null rest` rejects both a second operation and trailing letters. In particular, integer division makes `eval "34/4" = Just 8`. As permitted by the question, division by zero is outside the specified inputs; the bounded-`Int` proviso also applies to arithmetic results.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
