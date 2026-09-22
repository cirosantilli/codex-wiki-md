<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Search as for insertion. Removing a node with at most one nonempty child leaves that child in its place. With two children, use the smallest key in the right subtree as the replacement and remove that occurrence from the right subtree:

```
delete :: Ord a => a -> STree a -> STree a
delete _ Empty = Empty
delete y (Node left x right) =
  case compare y x of
    LT -> Node (delete y left) x right
    GT -> Node left x (delete y right)
    EQ -> join left right
  where
    -- Join two search trees with every left key below every right key.
    join :: STree a -> STree a -> STree a
    join Empty r = r
    join l Empty = l
    join l r = let (smallest, rest) = takeMin r
               in Node l smallest rest

-- Precondition: the input tree is nonempty.
takeMin :: STree a -> (a, STree a)
takeMin Empty = error "takeMin: empty tree"
takeMin (Node Empty x right) = (x, right)
takeMin (Node left x right) =
  let (smallest, rest) = takeMin left
  in (smallest, Node rest x right)
```

The call to `takeMin` occurs only after both empty cases have been excluded. Its [structural recursion](../../../../../structural-recursion.md) follows left children until it reaches the minimum label and rebuilds the path with that occurrence removed.

For a matching label $x$ and successor $s$, all left labels are below $x<s$, while every label remaining on the right is strictly above $s$. Thus replacing $x$ by $s$ preserves the [binary search tree](../../../../../binary-search-tree.md) invariant. Every other branch preserves the invariant by [structural induction](../../../../../structural-induction.md). The resulting [set](../../../../../set-split.md) is exactly

$$
\boxed{\operatorname{keys}(\operatorname{delete}\ y\ t)=\operatorname{keys}(t)\setminus\{y\}.}
$$

Whether the key is absent or present, untouched subtrees can be shared. The search path followed by the successor path uses $O(h)$ time and fresh nodes for original [height of a binary tree](../../../../../height-of-a-binary-tree.md) $h$, so the worst case is $O(n)$ without balancing. This is [persistent binary search tree deletion](../../../../../persistent-binary-search-tree-deletion.md): the original value remains available.

## ↑ Ancestors (12)

1. [G](../g.md)
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
