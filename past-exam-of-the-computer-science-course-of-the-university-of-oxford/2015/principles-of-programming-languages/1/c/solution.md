<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Reading preserves the [computer memory](../../../../../computer-memory-split.md); writing returns the [unit type](../../../../../unit-type.md) value; allocating returns both the fresh [memory location](../../../../../memory-location.md) and the allocator's updated [computer memory](../../../../../computer-memory-split.md):

```
get :: Monad m => Location -> MemT m Value
get a s = resultM (contents s a,s)

put :: Monad m => Location -> Value -> MemT m ()
put a v s = resultM ((),update s a v)

new :: Monad m => MemT m Location
new s = resultM (fresh s)
```

These use the memory interface in [Printed p. 3, Figure 1](../../../../../principles-of-programming-languages-examination-paper-by-the-university-of-oxford-2015.md). In particular, `fresh` already returns its outputs in the order required by the [state monad transformer](../../../../../state-monad-transformer.md):

$$
\boxed{\begin{aligned}
\operatorname{get}(a)\,s&=r_m(\operatorname{contents}(s,a),s),\\
\operatorname{put}(a,v)\,s&=r_m((),\operatorname{update}(s,a,v)),\\
\operatorname{new}\,s&=r_m(\operatorname{fresh}(s)).
\end{aligned}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
