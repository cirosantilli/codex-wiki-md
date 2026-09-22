<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**Yes, under the finite total assumption in part (d).** The pair result retains enough information to reconstruct the tail; the `~` pattern keeps its two components lazy:
```
spanFold :: (a -> Bool) -> [a] -> ([a], [a])
spanFold p = foldr step ([], [])
  where
    step x ~(ys,zs)
      | p x       = (x:ys,zs)
      | otherwise = ([],x:(ys ++ zs))
```
Take $f=\operatorname{spanP}\ p$, $g=(:)$ and $a=[]$. The base image is $([],[])$. If $p(x)$ is true, the recursive equation gives the first branch. If it is false, part (d), applied to the tail, gives $ys\mathbin{++}zs=xs$, so the second branch becomes $([],x:xs)$. These are precisely the fusion compatibility equations. Finite [structural induction](../../../../../structural-induction.md) establishes the desired equality; it does not require extending the restricted-domain hypothesis to undefined [predicate](../../../../../predicate.md) applications.

The qualification matters. If $p(v)$ is false but $p(u)$ is undefined, ordinary `spanP p [v,u]` can return the untouched [list suffix](../../../../../suffix-of-a-list.md) immediately, whereas the reconstruction through `spanFold p [u]` cannot recover that [list suffix](../../../../../suffix-of-a-list.md). The weaker condition needed only for the single reconstruction identity in (d) is therefore insufficient for this particular [list fold](../../../../../list-fold.md) on all [list suffixes](../../../../../suffix-of-a-list.md). The stronger totality condition stated there supplies exactly the missing premise.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
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
