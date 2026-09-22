<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Pass an already constructed suffix through the traversal:
```
convert :: Expr -> RPolish
convert e = go e []
  where
    go :: Expr -> RPolish -> RPolish
    go (Num n) rest = Number n : rest
    go (App op left right) rest =
      go left (go right (Operator op : rest))
```
The invariant is that `go e rest` is the [reverse Polish notation](../../../../../reverse-polish-notation.md) of `e` followed by `rest`. It holds at a numeric leaf. At an application, the result is the left subtree's tokens, then the right subtree's tokens, then the operator, then `rest`, exactly as required.

Each [vertex](../../../../../vertex-graph-theory.md) of the [abstract syntax tree](../../../../../abstract-syntax-tree.md) creates one output [list](../../../../../list-abstract-data-type.md) cell and performs constant local work. Thus producing the complete result takes **$O(n)$ time** for an expression with $n$ vertices. No repeated [list concatenation](../../../../../list-concatenation.md) copies a previously traversed subtree. This suffix-passing construction is a [difference list](../../../../../difference-list.md) traversal.

## ↑ Ancestors (12)

1. [B](../b.md)
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
