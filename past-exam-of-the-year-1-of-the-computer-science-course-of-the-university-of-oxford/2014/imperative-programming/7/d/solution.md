<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The rightmost [trait](../../../../../trait.md) intercepts insertion first. In `A`, capitalization runs before counting, so the counter receives uppercase `A` and does not increment the lowercase count. In `B`, counting receives lowercase `a`, delegates to capitalization, and then increments the original lowercase argument's counter. Both concrete documents store uppercase `A`.

The exact output is
```
0
1
```


$$
\boxed{d1.\mathrm{getCount}(\texttt{'a'})=0,\qquad d2.\mathrm{getCount}(\texttt{'a'})=1.}
$$

This illustrates an order-sensitive [stackable trait modification](../../../../../stackable-trait-modification.md). In the second composition the cached count describes intercepted insertion arguments, and no longer the actual lowercase characters in the stored document. For example, deleting its uppercase `A` would not decrement the lowercase counter. A counter required to track actual contents under arbitrary transforming [mixins](../../../../../mixin.md) would need a stronger composition contract or would inspect the stored character after insertion; such a change would alter the intended behavior of this example.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
