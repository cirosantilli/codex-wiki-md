<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Fix an answer type and let the [continuation](../../../../../continuation-computer-science.md) return its answer inside the base [computational monad](../../../../../computational-monad.md):

```
type ContT m a = (a -> m Answer) -> m Answer

result :: Monad m => a -> ContT m a
result x k = k x

bind :: Monad m => ContT m a -> (a -> ContT m b) -> ContT m b
bind p f k = p (\x -> f x k)
```

The [continuation monad transformer](../../../../../continuation-monad-transformer.md) changes the [continuation](../../../../../continuation-computer-science.md) supplied to `p`: it first runs `f` on the produced value, then uses the original final [continuation](../../../../../continuation-computer-science.md) `k`. Base sequencing is unnecessary in these two definitions because `p` already accepts a [continuation](../../../../../continuation-computer-science.md) returning `m Answer`. The customary lift, if desired, is `lift q k = bindM q k`.

$$
\boxed{\begin{aligned}
\operatorname{ContT}\ m\ A&=(A\to m\operatorname{Answer})\to m\operatorname{Answer},\\
\operatorname{result}(x)\,k&=k(x),\\
(p\triangleright f)\,k&=p(\lambda x.\,f(x)\,k).
\end{aligned}}
$$

## ↑ Ancestors (11)

1. [G](../g.md)
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
