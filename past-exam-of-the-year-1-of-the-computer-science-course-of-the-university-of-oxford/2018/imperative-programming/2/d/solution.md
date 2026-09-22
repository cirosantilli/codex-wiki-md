<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Black-box testing](../../../../../black-box-testing.md) chooses inputs and expected outputs from the public specification without using the implementation's control structure. [Equivalence class testing](../../../../../equivalence-partitioning.md) partitions the input space into classes expected to exercise similar specified behavior, then chooses representatives; boundary cases test where that behavior changes. For [equal-range search](../../../../../equal-range-search.md), use these concrete representatives:

- Empty [array](../../../../../array-data-structure.md): `([], 4)` gives **`(0,0)`**.
- One entry, with the target below, equal, and above it: `([4],3)`, `([4],4)`, `([4],5)` give **`(0,0)`, `(0,1)`, `(1,1)`**.
- An absent interior value: `([1,3,5],4)` gives **`(2,2)`**.
- One interior match: `([1,3,5],3)` gives **`(1,2)`**.
- A repeated interior block: `([1,3,3,3,5],3)` gives **`(1,4)`**.
- A repeated block touching the left or right boundary: `([3,3,5],3)` and `([1,3,3],3)` give **`(0,2)`** and **`(1,3)`**.
- Every entry equal: `([3,3,3],3)` gives **`(0,3)`**; targets two and four give **`(0,0)`** and **`(3,3)`**.
- Extreme keys: `([Int.MinValue,0,Int.MaxValue],Int.MaxValue)` gives **`(2,3)`**, and searching for `Int.MinValue` gives **`(0,1)`**.

For each result independently check $0\leq i\leq j\leq n$, the strict inequalities outside the returned interval, and equality inside it. Unsorted inputs violate the [precondition](../../../../../precondition.md); they are not ordinary members of the specified valid-input classes. [Software testing](../../../../../software-testing.md) supplies evidence about implementations, while the [loop invariant](../../../../../loop-invariant.md) proof explains correctness for every valid input.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
