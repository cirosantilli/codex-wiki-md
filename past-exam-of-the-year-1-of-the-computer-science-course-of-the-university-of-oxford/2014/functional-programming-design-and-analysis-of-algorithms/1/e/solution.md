<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Keep the two adjacent [Fibonacci numbers](../../../../../fibonacci-number.md) in one shared pair. From the [Fibonacci recurrence](../../../../../fibonacci-recurrence.md), if the current pair is $(F_n,F_{n+1})$, the next is $(F_{n+1},F_n+F_{n+1})$. This gives the [paired Fibonacci recurrence](../../../../../paired-fibonacci-recurrence.md):

```
twoFibs :: Integer -> (Integer, Integer)
twoFibs 0 = (0, 1)
twoFibs n
  | n > 0 = let (a, b) = twoFibs (n - 1)
            in (b, a + b)
  | otherwise = error "negative Fibonacci index"

fib :: Integer -> Integer
fib = fst . twoFibs
```

The pair pattern shares the result of the single [recursive call](../../../../../recursive-call.md). [Mathematical induction](../../../../../mathematical-induction.md) establishes

$$
\boxed{\operatorname{twoFibs}(n)=(F_n,F_{n+1}),\qquad \operatorname{fib}(n)=F_n.}
$$

There are $n$ pair updates and $n$ [additions](../../../../../addition.md), rather than the repeated subcomputations of the original branching [recursion](../../../../../recursion-computer-science.md). This is linear arithmetic-operation count; exact [Fibonacci numbers](../../../../../fibonacci-number.md) have growing bit length. The pattern `fib (n+2)` in the source expresses the recurrence; the guarded definition above uses ordinary [Haskell](../../../../../haskell.md) syntax without requiring an `n+k` pattern extension.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
