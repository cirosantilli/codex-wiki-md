<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use `concat [] = []`, `concat (ys:yss) = ys ++ concat yss`, the corresponding equations for `map`, [associativity](../../../../../associative-property.md) of [list concatenation](../../../../../list-concatenation.md), and `(r:ys) ++ zs = r:(ys ++ zs)`. For an empty forest,
```
flatten2 [] xs
= concat (map flatten []) ++ xs
= [] ++ xs
= xs
```
For a nonempty forest, write its first [rose tree](../../../../../rose-tree.md) as `Node r children`:
```
flatten2 (Node r children : trees) xs
= (flatten (Node r children) ++ concat (map flatten trees)) ++ xs
= (r : concat (map flatten children))
    ++ (concat (map flatten trees) ++ xs)
= r : (concat (map flatten children) ++ flatten2 trees xs)
= r : flatten2 children (flatten2 trees xs)
```
Thus the recursive [Haskell](../../../../../haskell.md) definition is
```
flatten2 :: [RTree a] -> [a] -> [a]
flatten2 [] xs = xs
flatten2 (Node r children : trees) xs =
  r : flatten2 children (flatten2 trees xs)
```
The nested call supplies the continuation of the [preorder traversal](../../../../../preorder-traversal.md) as a suffix. **Each label is emitted once**, without repeated [list concatenation](../../../../../list-concatenation.md) of an already flattened subtree. For a finite forest, constructing its entire contribution takes linear time in its number of [vertices](../../../../../vertex-graph-theory.md), without traversing the supplied suffix `xs`.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
