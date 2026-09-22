<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Separate the maximal decimal prefix from the unconsumed suffix, rejecting an empty prefix:
```
import Data.Char (isDigit, digitToInt)

type Parse a = String -> Maybe (a,String)

parseInt :: Parse Int
parseInt input =
  case span isDigit input of
    ([],_)  -> Nothing
    (ds,ys) -> Just (foldl (\n d -> 10*n + digitToInt d) 0 ds, ys)
```
The [left fold](../../../../../left-fold.md) uses the [positional notation](../../../../../positional-notation.md) recurrence $N_{j+1}=10N_j+d_j$. This parses unsigned decimal operands as illustrated, leaving the first nondigit and everything after it untouched. As the required result type is `Int`, correct mathematical values require the parsed integer to fit that bounded type; arbitrary-length exact values would instead need `Integer` or an explicit [integer overflow](../../../../../integer-overflow.md) check.

## ↑ Ancestors (12)

1. [C](../c.md)
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
