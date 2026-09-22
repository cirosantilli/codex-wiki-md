<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**`tails` is not a direct [list fold](../../../../../list-fold.md).** Every `foldr c z` is strict in its list argument, but `tails undefined = undefined : undefined` has a defined outer constructor. Applying `null` distinguishes this result from $\bot$.

**`ptails` is not a direct [list fold](../../../../../list-fold.md) either.** On a type with distinct values `u` and `v`,

$$
\operatorname{ptails}[u]=[[]]=\operatorname{ptails}[v].
$$

A fold step given the same new head `x` and these equal folded tails must return the same result. However,

$$
\operatorname{ptails}[x,u]=[[u],[]]\ne[[v],[]]=\operatorname{ptails}[x,v].
$$

Thus the tail information needed by the next step does not factor through `ptails`; this violates the [fold factorisation criterion](../../../../../fold-factorisation-criterion.md) even on finite total lists.

**`ntails` is a direct [list fold](../../../../../list-fold.md):**
```
ntailsFold :: [a] -> [[a]]
ntailsFold = foldr step []
  where
    step x yss = (x : original yss) : yss
    original [] = []
    original (ys:_) = ys
```
When the tail is nonempty, its first nonempty [suffix of a list](../../../../../suffix-of-a-list.md) is the tail itself; otherwise it is recovered as `[]`. Hence `original (ntailsFold xs) = xs`. The inner case distinction is delayed beneath constructors, so the definition also preserves the required behaviour on partial and infinite [lazy lists](../../../../../lazy-list.md). Building a suffix head does not first demand the whole folded tail.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
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
