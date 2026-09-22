<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [Scala trait linearization](../../../../../scala-trait-linearization.md), the rightmost mixed-in [trait](../../../../../trait.md) takes priority. Merge inherited linearizations while retaining a shared ancestor only at its final position; `super` advances to the next implementation in the resulting chain. Ignoring predefined bases, the lookup orders are
```
Life1, Exercise, Work, Life
Life2, Dance, Exercise, Program, Study, Work, Fun, Life
Life3, Program, Study, Work, Dance, Fun, Exercise, Life
```
For example, `Dance` alone has order `Dance, Fun, Exercise, Life`. In `Life2`, the additional `Program` branch already contains `Fun` before `Life`; keeping that shared ancestry in its later position moves `Fun` after `Work`, while `Dance` still takes priority. Reversing the mixins yields the third chain above.

Each `describe` first delegates and then prints, so the lines appear in the reverse of the method lookup order. The exact output, including the two blank lines, is
```
I live.
I work.
I exercise.

I live.
I have fun.
I work.
I study.
I program.
I exercise.
I dance.

I live.
I exercise.
I have fun.
I dance.
I work.
I study.
I program.
```


$$
\boxed{\text{Lookup follows the linearization; these prints occur while the calls return}.}
$$

The `super` inside a [trait](../../../../../trait.md) therefore need not call that [trait](../../../../../trait.md)'s isolated textual parent; the receiving object's full [Scala trait linearization](../../../../../scala-trait-linearization.md) controls the next body.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
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
