<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

List each [Scala trait linearization](../../../../../scala-trait-linearization.md) from the most specific [software class](../../../../../class-programming.md) toward the common base, omitting predefined types:
```
Life1, Party, Study, Life
Life2, Sport, Exercise, Research, Party, Study, Life
Life3, Research, Study, Sport, Party, Exercise, Life
```
For example, `Sport` alone linearizes as `Sport, Party, Exercise, Life`, while `Research` alone gives `Research, Party, Study, Life`. In combining parents, take the right parent's linearization first, deleting from it entries also present in the remaining left-parent linearization, then append the latter. This places a common base after all of its derived [traits](../../../../../trait.md).[Class Linearization](../../../../../scala-2-11-classes-and-objects-specification.md)

An unqualified `super.describe()` continues after the current [trait](../../../../../trait.md) in the actual receiver's [Scala trait linearization](../../../../../scala-trait-linearization.md). Each override prints after its `super` call, so the output follows the displayed order backwards, starting at `Life`. The complete output is:
```
I live.
More on study.
More on party.
I live.
More on study.
More on party.
More on research.
More on exercise.
More on sport.
I live.
More on exercise.
More on party.
More on sport.
More on study.
More on research.
```
The first three lines belong to `l1`, the next six to `l2`, and the final six to `l3`.

$$
\boxed{\text{Rightmost mixin has lookup priority; super-first printing reverses the lookup chain}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
