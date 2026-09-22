<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use an auxiliary [parser](../../../../../parser.md) that returns both a value and the unconsumed suffix. The arithmetic helper is:
```
applyOp :: Op -> Int -> Int -> Int
applyOp Add x y = x + y
applyOp Sub x y = x - y
applyOp Mul x y = x * y
applyOp Div x y = x `div` y
```
For the integer-valued expression language, this chooses [integer division](../../../../../integer-division.md) with `div`'s rounding convention. The result is evaluated under the intended arithmetic model; bounded-`Int` overflow is separate from parsing.
```
evalP :: Polish -> Int
evalP input =
  case parse input of
    (value, []) -> value
    _           -> error "trailing tokens"
  where
    parse :: Polish -> (Int, Polish)
    parse [] = error "missing operand"
    parse (Number n : rest) = (n, rest)
    parse (Operator op : rest) =
      let (left, rest1)  = parse rest
          (right, rest2) = parse rest1
      in (applyOp op left right, rest2)
```
A number consumes one token. An operator consumes the two successive complete expressions that follow it, so nested operators are handled by [recursion](../../../../../recursion-computer-science.md). [Structural induction](../../../../../structural-induction.md) on the expression proves that `parse` consumes exactly its [Polish notation](../../../../../polish-notation.md) and returns its value. Keeping the suffix is essential: neither operand has a fixed token count. Division by zero need not be treated separately under the stated input convention.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
