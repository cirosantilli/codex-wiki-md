<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [list concatenation](../../../../../list-concatenation.md) as the combining operation and the empty [list](../../../../../list-abstract-data-type.md) as the seed:

```
concat :: [[a]] -> [a]
concat = foldr (++) []
```

For three inner [lists](../../../../../list-abstract-data-type.md), this constructs `xs ++ (ys ++ (zs ++ []))`, preserving the elements' original order. The concise answer is $\boxed{\operatorname{concat}=\operatorname{foldr}\,(\mathbin{+\!+})\,[\,]}$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
