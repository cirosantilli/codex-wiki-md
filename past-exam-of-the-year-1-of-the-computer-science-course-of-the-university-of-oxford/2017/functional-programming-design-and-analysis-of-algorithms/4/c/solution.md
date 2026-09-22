<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use `map k (u:us) = k u : map k us`, list-map fusion, and the [left fold](../../../../../left-fold.md) equation

```
foldl f e (x:ys) = foldl f (f e x) ys
```

For the empty list, the prefix definition immediately gives `scanl f e [] = [e]`. For a nonempty list, calculate:

```
scanl f e (x:xs)
  = map (foldl f e) ([] : map (x:) (inits xs))
  = e : map ((foldl f e) . (x:)) (inits xs)
  = e : map (foldl f (f e x)) (inits xs)
  = e : scanl f (f e x) xs
```

The second-to-third line uses the displayed fold equation as an equality of functions of `ys`. Hence the efficient [left scan](../../../../../left-scan.md) is:

```
scanl :: (b -> a -> b) -> b -> [a] -> [b]
scanl f e [] = [e]
scanl f e (x:xs) = e : scanl f (f e x) xs
```

On a finite input of length $n$, fully demanding the original prefix-fold results performs $0+1+\cdots+n=n(n+1)/2$ accumulator updates. The recurrence performs $n$. Thus the update count improves from **$\Theta(n^2)$ to $\Theta(n)$**, assuming constant-cost updates. Both return $n+1$ results. This does not assert constant space for arbitrary accumulators or imply that lazy accumulators are evaluated strictly.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
