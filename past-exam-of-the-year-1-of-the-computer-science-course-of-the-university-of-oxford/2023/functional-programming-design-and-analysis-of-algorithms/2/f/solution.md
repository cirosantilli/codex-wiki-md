<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**For finite, fully defined representations, yes; for arbitrary infinite ones in [Haskell](../../../../../haskell.md), no.** At the level of mathematical occurrence sets, splitting by parity, dividing by two, and then applying the inverse index transformations recovers every original position exactly once. Thus the equality holds on finite total position lists.

For a proper infinite representation, take the alternating Boolean sequence, represented by
```
alternating :: Seq Bool
alternating False = [0,2..]
alternating True = [1,3..]
```
This is a total representation: both queries return productive infinite occurrence lists. But
```
odds alternating False
```
filters for odd indices in `[0,2..]`, so it produces no outer constructor and denotes $\bot$. The call
```
ilv (evens alternating) (odds alternating) False
```
uses `mergePos` to inspect both transformed lists before emitting its first result; it therefore also diverges. In contrast, `alternating False` starts with `0`. Applying `head` distinguishes the two. The [productivity](../../../../../stream-productivity.md) failure is real even though the mathematical position-set identity is correct; the hypothesis that the input properly represents an infinite sequence does not remove it.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
