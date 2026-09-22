<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Use the input [list](../../../../../list-abstract-data-type.md) as the seed of the [tree unfold](../../../../../tree-unfold.md):

```
buildUnfold :: [a] -> Tree a
buildUnfold = unfold step
  where
    step []  = error "build: empty input"
    step [x] = Left x
    step xs  = Right (split (length xs `div` 2) xs)
```

On a singleton seed, `unfold` produces the same leaf as `build`; on a longer finite seed, it recursively builds the same two pieces. [Induction](../../../../../mathematical-induction.md) on input length proves **`buildUnfold = build` on finite nonempty inputs**. The empty-input qualification remains essential: a [tree unfold](../../../../../tree-unfold.md) cannot supply a missing empty-tree constructor.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
