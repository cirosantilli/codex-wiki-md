<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Collect the matching replacements and distinguish all three possible multiplicities:
```
applyRule :: [Rule] -> Char -> String
applyRule rules c =
  case [replacement | (key, replacement) <- rules, key == c] of
    []          -> error ("no rule for " ++ [c])
    [result]    -> result
    (_:_:_)     -> error ("multiple rules for " ++ [c])
```
The [list comprehension](../../../../../list-comprehension.md) selects precisely the rules whose left-hand character is `c`. A singleton is the required unique match. The third branch also rejects duplicate rules with identical right-hand sides: there are still two matching rules. Finiteness of the rule list makes the uniqueness test decidable. The returned replacement may itself be empty.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
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
