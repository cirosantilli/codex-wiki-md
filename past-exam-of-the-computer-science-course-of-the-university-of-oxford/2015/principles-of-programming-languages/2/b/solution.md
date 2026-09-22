<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the memory interface before invoking the supplied [continuation](../../../../../continuation-computer-science.md):

```
get :: Location -> M Value
get a k s = k (contents s a) s

put :: Location -> Value -> M ()
put a v k s = k () (update s a v)

new :: M Location
new k s = let (a,s') = fresh s in k a s'
```

A read preserves [computer memory](../../../../../computer-memory-split.md); a write changes it but returns the [unit type](../../../../../unit-type.md) value; an allocation uses the updated [computer memory](../../../../../computer-memory-split.md) returned by `fresh`. The [continuation](../../../../../continuation-computer-science.md) always receives the latest [computer memory](../../../../../computer-memory-split.md):

$$
\boxed{\begin{aligned}
\operatorname{get}(a)\,k\,s&=k(\operatorname{contents}(s,a))\,s,\\
\operatorname{put}(a,v)\,k\,s&=k(())(\operatorname{update}(s,a,v)),\\
\operatorname{new}\,k\,s&=k(a)\,s'\quad\text{where }(a,s')=\operatorname{fresh}(s).
\end{aligned}}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
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
