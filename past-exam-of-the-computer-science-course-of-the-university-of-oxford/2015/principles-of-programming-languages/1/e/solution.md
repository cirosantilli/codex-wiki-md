<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [identity monad](../../../../../identity-monad.md) embeds a value unchanged and sequences by ordinary application:

```
type IdM a = a
result :: a -> IdM a
result x = x
bind :: IdM a -> (a -> IdM b) -> IdM b
bind x f = f x
```

All three [monad laws](../../../../../monad-laws.md) reduce to substitution in [function](../../../../../function-split.md) application. There is no additional [program state](../../../../../program-state.md), failure alternative or [continuation](../../../../../continuation-computer-science.md) layer:

$$
\boxed{\operatorname{result}(x)=x,\qquad x\triangleright f=f(x).}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
