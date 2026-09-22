<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The following shared step consumes exactly one input element per recursive call of `group1`:
```
prependRun :: Eq a => a -> [[a]] -> [[a]]
prependRun x xss = (x:same):rest
  where
    ~(same,rest) = case xss of
      [] -> ([],[])
      run@(y:_):runs
        | x == y    -> (run,runs)
        | otherwise -> ([],xss)

group1 :: Eq a => [a] -> [[a]]
group1 []     = []
group1 (x:xs) = prependRun x (group1 xs)
```
The helper's input consists of nonempty runs. If its first run starts with `x`, prepend `x` to that run; otherwise create a new singleton run. [Structural induction](../../../../../structural-induction.md) proves that these are the maximal equal runs in order. The irrefutable pair binding `~(same,rest)` preserves [lazy evaluation](../../../../../lazy-evaluation.md): the first output group exposes its initial `x` without inspecting the recursively grouped tail. Thus even an infinite constant input can expose the first group and each finite prefix of that group. Finite inputs take [linear time](../../../../../linear-time.md) when [equality tests](../../../../../equality-test.md) take [constant time](../../../../../constant-time.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
