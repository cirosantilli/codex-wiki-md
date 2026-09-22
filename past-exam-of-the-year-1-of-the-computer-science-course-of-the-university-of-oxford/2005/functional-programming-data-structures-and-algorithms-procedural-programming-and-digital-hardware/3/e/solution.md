<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For two [proper lazy lists](../../../../../proper-lazy-list.md), `twiddle` alternates heads, swapping which [list](../../../../../list-abstract-data-type.md) is served after each output. Thus both input positions have finite waiting time. A tempting extension is `remalldups . foldr twiddle []`, but arbitrary empty rows make that insufficient: for `[ [1,2] ] ++ repeat []`, it emits `1` and then demands the combination of infinitely many empty rows before it can return to `2`.

Use [diagonal merging of lazy lists](../../../../../diagonal-merging-of-lazy-lists.md) to avoid that obstruction. Maintain a finite active collection, add at most one new row per round, and take one head from every nonempty active row. The supplied `twiddle` combines those singleton contributions into a finite batch:

```
union' = remalldups . rounds []

rounds [] [] = []
rounds active [] = emit active []
rounds active (row:rows) = emit (active ++ [row]) rows

emit active rows = batch ++ rounds tails rows
  where (batch, tails) = sweep active

sweep [] = ([], [])
sweep ([]:rows) = sweep rows
sweep ((x:xs):rows) = (twiddle [x] heads, xs:tails)
  where (heads, tails) = sweep rows
```

Here `rounds` takes the finite active collection first and the not-yet-introduced outer [list](../../../../../list-abstract-data-type.md) second. Because `heads` is a finite [list](../../../../../list-abstract-data-type.md), `twiddle [x] heads` emits `x` followed by those heads; the finite batch is then completely consumed before the next round. Empty exhausted rows are removed by `sweep`. No step tries to combine infinitely many not-yet-introduced rows.

Index rows and positions from zero. Row $i$ is introduced in round $i$ and contributes its element $j$ in round $i+j$, if that element exists. Every earlier round inspects only finitely many rows. Therefore every occurrence has a finite emission time, proving [fair enumeration](../../../../../fair-enumeration.md). Applying [first-occurrence duplicate removal](../../../../../first-occurrence-duplicate-removal.md) gives

$$
\boxed{\operatorname{union}'=\operatorname{remalldups}\circ\text{finite-round diagonal enumeration}.}
$$

All outer and inner spines must be [proper lazy lists](../../../../../proper-lazy-list.md) and [equality tests](../../../../../equality-test.md) must terminate. Infinitely many empty rows after the final contribution still prevent certifying a terminating empty tail, just as part (c) predicts. Undefined input spines have the separate [partial-list interleaving obstruction](../../../../../partial-list-interleaving-obstruction.md); the construction makes no promise to bypass them.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
