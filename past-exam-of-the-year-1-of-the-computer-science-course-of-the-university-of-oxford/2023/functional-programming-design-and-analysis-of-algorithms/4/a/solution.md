<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the source's constructor order: left subtree, root value, right subtree.
```
data Tree a = Tree (Tree a) a (Tree a) | Empty

foldTree :: (b -> a -> b -> b) -> b -> Tree a -> b
foldTree node empty Empty = empty
foldTree node empty (Tree l x r) =
  node (foldTree node empty l) x (foldTree node empty r)

unfoldTree :: (s -> Maybe (s,a,s)) -> s -> Tree a
unfoldTree next seed = case next seed of
  Nothing -> Empty
  Just (ls,x,rs) ->
    Tree (unfoldTree next ls) x (unfoldTree next rs)
```
A [tree fold](../../../../../tree-fold.md) replaces the two constructors by an algebra on already folded children. A [tree unfold](../../../../../tree-unfold.md) expands a seed either into the empty tree or into a root value and two new seeds. The definitions themselves work on arbitrary binary trees; preserving the [binary search tree](../../../../../binary-search-tree.md) ordering requires the supplied algebra or seed expansion to respect its bounds.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
