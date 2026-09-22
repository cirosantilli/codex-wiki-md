<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

A [tree fold](../../../../../tree-fold.md) can compute insertion while retaining the unchanged children by carrying a pair. The following fold-derived implementation preserves the [lazy evaluation](../../../../../lazy-evaluation.md) behaviour of part (f):
```
insertViaFold :: Ord a => a -> Tree a -> Tree a
insertViaFold q t = snd (foldTree node base t)
  where
    base = (Empty, Tree Empty q Empty)
    node ~(l,li) x ~(r,ri) = (original,updated)
      where
        original = Tree l x r
        updated = case compare q x of
          LT -> Tree li x r
          EQ -> original
          GT -> Tree l x ri
```
The [invariant](../../../../../invariant-mathematics.md) of the folded pair is `(original subtree, subtree with q inserted)`. The empty case establishes it. At a node, the first components reconstruct the original tree, and the second components supply whichever child insertion is needed. The irrefutable pair patterns `~(l,li)` and `~(r,ri)` avoid demanding an unused child's fold. Induction on finite approximations therefore proves equivalence even for partial trees, and only the selected search route needs insertion work.

There is a distinction if “written as a fold” is required to mean a direct same-result-type expression `insert q = foldTree node base`, with no richer result and final projection. On finite fully defined [binary search trees](../../../../../binary-search-tree.md), such an expression is possible by [undoing insertion of a new extreme key](../../../../../undoing-insertion-of-a-new-extreme-key.md) in the child that should remain unchanged. For completeness, a literal direct fold on that finite, fully defined domain is:
```
eraseFresh :: Ord a => a -> Tree a -> Tree a
eraseFresh _ Empty = Empty
eraseFresh q (Tree l x r) = case compare q x of
  LT -> Tree (eraseFresh q l) x r
  EQ -> Empty
  GT -> Tree l x (eraseFresh q r)

insertDirectFold :: Ord a => a -> Tree a -> Tree a
insertDirectFold q = foldTree node (Tree Empty q Empty)
  where
    node left x right = case compare q x of
      LT -> Tree left x (eraseFresh q right)
      EQ -> Tree (eraseFresh q left) x (eraseFresh q right)
      GT -> Tree (eraseFresh q left) x right
```
Here `eraseFresh` is used only to undo a newly inserted extreme key, which is a leaf; it is not a general deletion operation. The [binary search tree](../../../../../binary-search-tree.md) bound at each root guarantees exactly that precondition on every child being restored.

On all partial [Haskell](../../../../../haskell.md) trees, however, a direct expression with result type `Tree a` cannot implement part (f).

For that obstruction, fix `q = 0`, and consider the two right subtrees
```
r1 = Tree Empty undefined Empty
r2 = Tree Empty undefined (Tree Empty 3 Empty)
```
Both can be completed to valid right subtrees of a root labelled `1`. Yet `insert 0 r1` and `insert 0 r2` are both bottom, because insertion must compare `0` with their undefined root label. A direct fold equal to insertion would therefore receive the same folded left value, root `1`, and bottom folded right value on both larger trees `Tree Empty 1 r1` and `Tree Empty 1 r2`. It must return the same result. Part (f) instead preserves `r1` or `r2`, which are distinguishable by inspecting their right-child constructors without inspecting the undefined labels. This proves the direct-fold obstruction. The pair-valued implementation avoids losing that information and states precisely which sense of fold implementation is being used.

## ↑ Ancestors (12)

1. [G](../g.md)
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
