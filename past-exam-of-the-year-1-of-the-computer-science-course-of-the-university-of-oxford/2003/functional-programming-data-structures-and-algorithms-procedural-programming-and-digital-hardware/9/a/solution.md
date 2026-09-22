<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a least-significant-first [bit-serial comparator](../../../../../bit-serial-comparator.md), the new pair has higher significance than every pair already processed. Equal new [bits](../../../../../bit.md) preserve the earlier result; unequal new [bits](../../../../../bit.md) decide the new result regardless of earlier [bits](../../../../../bit.md). Use a [left fold](../../../../../left-fold.md) starting at equality:

```
type Bit = Int
data LEG = Lt | Eq | Gt deriving (Eq, Show)

step :: LEG -> (Bit,Bit) -> LEG
step old (a,b)
  | a < b = Lt
  | a > b = Gt
  | otherwise = old

compare :: [Bit] -> [Bit] -> LEG
compare as bs = foldl step Eq (pairs as bs)
  where
    pairs [] [] = []
    pairs (a:as) [] = (a,0) : pairs as []
    pairs [] (b:bs) = (0,b) : pairs [] bs
    pairs (a:as) (b:bs) = (a,b) : pairs as bs
```

Inputs have the [precondition](../../../../../precondition.md) that each `Bit` is `0` or `1`. Equal-length inputs are the physical circuit case; `pairs` also gives a defined unsigned meaning to unequal lengths by padding the shorter input with high-order zeros. Ordinary `zip` would silently discard significant unmatched [bits](../../../../../bit.md).

After $k$ pairs the [fold](../../../../../fold.md) accumulator compares $A_k=\sum_{i<k}a_i2^i$ and $B_k=\sum_{i<k}b_i2^i$. Equal new [bits](../../../../../bit.md) add the same amount. If $a_k\ne b_k$, the new difference has magnitude $2^k$, exceeding the maximum magnitude $2^k-1$ of the earlier difference. This proves the accumulator invariant and gives

$$
\boxed{\operatorname{compare}(as,bs)=\operatorname{foldl}\ \operatorname{step}\ \mathrm{Eq}\ (\operatorname{pairs}(as,bs)).}
$$

For the four pairs in the source, the states are `Lt, Gt, Gt, Lt`, so the final result compares $6<13$ correctly.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
