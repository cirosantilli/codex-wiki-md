<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set both $\oplus$ and $\otimes$ equal to [list concatenation](../../../../../list-concatenation.md), with $a=[]$. [Associativity](../../../../../associative-property.md) gives `xs ++ (ys ++ zs) = (xs ++ ys) ++ zs`, which is equation (1). The two identity laws give `xs ++ [] = [] ++ xs`, which is equation (2). Part (b) therefore yields

```
concat :: [[a]] -> [a]
concat = foldl (++) []
```

Thus $\boxed{\operatorname{concat}=\operatorname{foldl}\,(\mathbin{+\!+})\,[\,]}$ on finite [lists](../../../../../list-abstract-data-type.md). The argument order is unchanged: the accumulator is the already concatenated prefix, and the next inner [list](../../../../../list-abstract-data-type.md) is appended to its right. This preserves the order but repeatedly copies that prefix.

## ↑ Ancestors (12)

1. [D](../d.md)
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
