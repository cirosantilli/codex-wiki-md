<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [three-way quicksort](../../../../../three-way-quicksort.md) can use a common partition helper so that the tree factorisation below makes the same key comparisons. The `compare` operation is assumed to be a terminating lawful total ordering on the supplied keys.
```
partition3 :: Ord a => a -> [a] -> ([a],[a],[a])
partition3 pivot = foldr step ([],[],[])
  where
    step x rest =
      let (lo,eq,hi) = rest
      in case compare x pivot of
           LT -> (x:lo,eq,hi)
           EQ -> (lo,x:eq,hi)
           GT -> (lo,eq,x:hi)

sort :: Ord a => [a] -> [a]
sort [] = []
sort (pivot:xs) =
  let (lo,eq,hi) = partition3 pivot xs
  in sort lo ++ (pivot:eq) ++ sort hi
```
Every non-pivot entry appears in exactly one partition, and the equal bucket contains the original pivot exactly once. The recursive sublists have length at most one less than the current finite input, so [recursion](../../../../../recursion-computer-science.md) terminates. [Induction](../../../../../mathematical-induction.md) gives sorted recursive results with the original multiplicities; placing the equal bucket between them gives a sorted [permutation](../../../../../permutation.md) of the input. There is no [recursive call](../../../../../recursive-call.md) on the equal bucket, which avoids needless descent on repeated keys.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
