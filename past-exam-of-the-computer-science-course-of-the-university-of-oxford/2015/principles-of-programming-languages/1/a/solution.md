<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Thread the explicit [program state](../../../../../program-state.md) through the computation, using the base [computational monad](../../../../../computational-monad.md) to sequence its effects:

$$
\boxed{\begin{aligned}
\operatorname{result}(x)\,s&=r_m(x,s),\\
(p\triangleright f)\,s&=(p\,s)\triangleright_m\bigl(\lambda(x,s').\,f(x)\,s'\bigr).
\end{aligned}}
$$

In [Haskell](../../../../../haskell.md) notation, with `resultM` and `bindM` standing for the base operations:

```
result :: Monad m => a -> MemT m a
result x s = resultM (x,s)

bind :: Monad m => MemT m a -> (a -> MemT m b) -> MemT m b
bind p f s = bindM (p s) (\(x,s') -> f x s')
```

This is the [state monad transformer](../../../../../state-monad-transformer.md). The first computation's final [program state](../../../../../program-state.md), rather than its initial [program state](../../../../../program-state.md), becomes the second computation's input. The base [computational monad](../../../../../computational-monad.md) decides whether that pair is available at all.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Principles of programming languages](../../../principles-of-programming-languages-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
