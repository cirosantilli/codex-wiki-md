<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An empty constructor and a constructor containing a label and two subtrees give a [polymorphic](../../../../../programming-language-polymorphism.md) [algebraic data type](../../../../../algebraic-data-type.md):

```
data STree a = Empty | Node (STree a) a (STree a)
  deriving (Eq, Show)
```

The [binary search tree](../../../../../binary-search-tree.md) invariant is $\boxed{\text{every left label}<x<\text{every right label}}$ at each `Node left x right`, together with the same invariant recursively in both subtrees. Labels are distinct because the representation is of a [set](../../../../../set-split.md). The declaration itself needs no ordering constraint; operations that compare labels require `Ord a` in their [type signatures](../../../../../type-signature.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
