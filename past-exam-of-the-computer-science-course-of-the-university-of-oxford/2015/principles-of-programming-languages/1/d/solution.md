<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

There is one undifferentiated exception, so use the two alternatives of the [Haskell](../../../../../haskell.md) [algebraic data type](../../../../../algebraic-data-type.md) `Maybe`: `Just x` succeeds and `Nothing` fails. A suitable [exception monad transformer](../../../../../exception-monad-transformer.md) is:

```
type ExT m a = m (Maybe a)

result :: Monad m => a -> ExT m a
result x = resultM (Just x)

bind :: Monad m => ExT m a -> (a -> ExT m b) -> ExT m b
bind p f = bindM p (\r -> case r of
  Nothing -> resultM Nothing
  Just x  -> f x)

orelse :: Monad m => ExT m a -> ExT m a -> ExT m a
orelse p q = bindM p (\r -> case r of
  Nothing -> q
  Just x  -> resultM (Just x))

failure :: Monad m => ExT m a
failure = resultM Nothing
```

The distinction between `bindM` and `bind` matters. The handler must inspect the failed alternative using the base [computational monad](../../../../../computational-monad.md); the transformed `bind` would propagate failure without running that inspection. The alternative computation `q` runs only after `p` returns `Nothing`; any effects already performed by the base [computational monad](../../../../../computational-monad.md) remain subject to that base's semantics.

Left identity follows by selecting `Just x`. Right identity follows because either alternative is passed back to `resultM`. For [associativity](../../../../../associative-property.md), base [associativity](../../../../../associative-property.md) exposes the first alternative: `Nothing` propagates through both remaining steps; `Just x` runs `f x`, with its `Nothing` and `Just` alternatives treated identically on both sides. Thus this representation also satisfies the [monad laws](../../../../../monad-laws.md).

$$
\boxed{\operatorname{ExT}\ m\ A=m(\operatorname{Maybe}\ A),\qquad
\operatorname{failure}\mathbin{\operatorname{orelse}}q=q,\qquad
\operatorname{result}(x)\mathbin{\operatorname{orelse}}q=\operatorname{result}(x).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
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
