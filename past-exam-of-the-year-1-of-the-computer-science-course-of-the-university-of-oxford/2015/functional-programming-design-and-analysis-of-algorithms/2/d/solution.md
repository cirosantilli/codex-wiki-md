<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Maintain a [stack](../../../../../stack-data-structure.md) of values of the complete subexpressions encountered so far, with the newest value at its head:
```
evalRP :: RPolish -> Int
evalRP = finish . foldl push []
  where
    push :: [Int] -> Elem -> [Int]
    push stack (Number n) = n : stack
    push (right:left:stack) (Operator op) =
      applyOp op left right : stack
    push _ (Operator _) = error "missing operand"

    finish :: [Int] -> Int
    finish [value] = value
    finish _       = error "malformed expression"
```
The [left fold](../../../../../left-fold.md) processes tokens in their order. A number pushes its own value; an operator replaces the two latest subexpression values by their combination. The top value is the **right** operand, so preserving the order in `applyOp op left right` is necessary for [subtraction](../../../../../subtraction.md) and [division](../../../../../division-mathematics.md). Induction on the consumed token prefix proves this [stack machine](../../../../../stack-machine.md) invariant. A complete valid expression finishes with exactly one value.

## ↑ Ancestors (12)

1. [D](../d.md)
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
