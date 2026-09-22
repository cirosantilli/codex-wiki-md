<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Capturing a [continuation](../../../../../continuation-computer-science.md) retains the destination, while the [computer memory](../../../../../computer-memory-split.md) is supplied when that destination is eventually invoked. The required [Haskell](../../../../../haskell.md) definitions are:

```
callcc :: (Cont a -> M a) -> M a
callcc f k s = f k k s

withc :: Cont a -> M a -> M a
withc saved p _current s = p saved s

callccPrim :: [Value] -> M Value
callccPrim [Function f] =
  callcc (\k -> f [Continuation k])

withcPrim :: [Value] -> M Value
withcPrim [Continuation k,v] = withc k (result v)
```

In `callcc`, the handler `f k` initially runs with the same current [continuation](../../../../../continuation-computer-science.md) `k`. If it returns normally, its result goes there. If it invokes `withc` with a saved [continuation](../../../../../continuation-computer-science.md), the current destination is discarded. In particular,

$$
\boxed{\operatorname{callcc}(f)\,k\,s=f(k)\,k\,s,\qquad
\operatorname{withc}(k',p)\,k\,s=p\,k'\,s.}
$$

The primitive interface receives values, because the surrounding [call-by-value](../../../../../call-by-value.md) [interpreter](../../../../../interpreter-computing.md) has already evaluated its arguments. Thus the expression supplied as the second argument of `withc` is evaluated once, before `withcPrim` transfers its value. Wrapping that value with `result` implements precisely the remaining transfer; the primitive must not try to evaluate it a second time. Neither operation restores a saved snapshot of [computer memory](../../../../../computer-memory-split.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Principles of programming languages](../../../principles-of-programming-languages-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
