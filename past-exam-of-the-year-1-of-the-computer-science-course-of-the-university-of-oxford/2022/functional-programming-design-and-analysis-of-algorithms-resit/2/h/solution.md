<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Skip whole trees using their cached sizes, then descend through one tree:
```
index :: List a -> Int -> a
index (List ts) i
  | i < 0     = error "index: negative index"
  | otherwise = seek ts i
  where
    seek [] _ = error "index: out of bounds"
    seek ((w,t):us) j
      | j < w     = at w t j
      | otherwise = seek us (j-w)
    at _ (Leaf x) 0 = x
    at w (Node x l r) j
      | j == 0 = x
      | j <= h = at h l (j-1)
      | otherwise = at h r (j-1-h)
      where h = w `div` 2
    at _ _ _ = error "index: invalid representation"
```
After skipping a size-$w$ tree, the desired index decreases by $w$. Inside a node, position zero is the root, positions $1,\ldots,h$ belong to the left child and the following $h$ positions to the right child. This proves correctness by [structural induction](../../../../../structural-induction.md) on the search.

There are at most $\lceil\log_2(n+1)\rceil$ [forest](../../../../../forest.md) entries by the supplied bound, and each tree has logarithmic height. Consequently a valid query takes **$O(\log(n+1))$ time**, with logarithmic worst cases. On a conventional [linked list](../../../../../linked-list.md), `xs !! i` follows $i$ links and costs $\Theta(i+1)$, hence $\Theta(n)$ in the worst case. The first element remains a [constant time](../../../../../constant-time.md) query in either representation.

## ↑ Ancestors (12)

1. [H](../h.md)
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
