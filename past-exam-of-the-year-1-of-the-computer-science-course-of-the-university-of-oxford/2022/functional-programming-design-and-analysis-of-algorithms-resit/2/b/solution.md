<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [Haskell](../../../../../haskell.md) representation is:
```
import Prelude hiding (null, head, tail)

data RTree a = Leaf a | Node a (RTree a) (RTree a)
newtype List a = List [(Int, RTree a)]
```
Every tree stores a value at its root, including internal nodes. Interpret the [forest](../../../../../forest.md) by root-left-right [preorder traversal](../../../../../preorder-traversal.md), concatenating the results in [forest](../../../../../forest.md) order. Valid values have correct cached sizes, [perfect binary trees](../../../../../perfect-binary-tree.md), nondecreasing sizes and only the permitted initial duplicate. The raw constructors can express invalid representations, so the operations below assume valid values and should form the public interface. Sizes are assumed to fit in `Int`; the stated [time complexities](../../../../../time-complexity.md) use constant-time size arithmetic.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
