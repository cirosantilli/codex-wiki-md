<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For [prefixes of a list](../../../../../prefix-of-a-list.md), the corresponding [Haskell](../../../../../haskell.md) definitions are
```
inits :: [a] -> [[a]]
inits xs = [] : ninits xs

pinits :: [a] -> [[a]]
pinits [] = []
pinits (x:xs) = [] : map (x:) (pinits xs)

ninits :: [a] -> [[a]]
ninits [] = []
ninits (x:xs) = map (x:) (inits xs)
```
The empty prefix is available without inspecting the input in `inits`. Every nonempty [prefix of a list](../../../../../prefix-of-a-list.md) begins with its input's head, explaining the last equation. For `pinits (x:xs)`, prepend `x` only to proper prefixes of `xs`, and include the empty prefix.

On finite inputs, `inits [] = [[]]`, whereas both other functions return `[]`. On an infinite input, all finite prefixes are proper and these definitions produce them incrementally. Fully constructing all elements of all prefixes takes $\Theta(n^2)$ work for an input of length $n$, matching the size of that output; there are no repeated end-append operations to add another factor.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
