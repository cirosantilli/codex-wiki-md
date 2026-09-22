<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First remove a single matching token, so duplicates cannot be reused:
```
pluck :: Eq a => a -> [a] -> Maybe [a]
pluck _ [] = Nothing
pluck x (y:ys)
  | x == y = Just ys
  | otherwise = case pluck x ys of
      Nothing -> Nothing
      Just zs -> Just (y:zs)

overlap :: Eq a => [a] -> [a] -> [a]
overlap [] _ = []
overlap (x:xs) ys = case pluck x ys of
  Nothing -> overlap xs ys
  Just zs -> x : overlap xs zs

scoreBC :: Eq a => [a] -> [a] -> (Int,Int)
scoreBC secret guess = (bulls, matches - bulls)
  where
    bulls = length [() | (s,g) <- zip secret guess, s == g]
    matches = length (overlap guess secret)
```
Equal game lengths are assumed. For each token, `overlap` retains exactly the smaller of its two multiplicities, so its length is the [multiset overlap](../../../../../multiset-overlap.md). It never spends a secret occurrence twice. Positional matches account for `bulls`; after reserving them, each token's remaining possible matches decrease by exactly its bull count. Hence `matches - bulls` counts precisely the cows. The source example gives **`(1,1)`**. With equality as the only operation on tokens, these definitions take $O(L^2)$ time for length $L$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
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
