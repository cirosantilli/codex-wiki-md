<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each row, keep the [row run length](../../../../../row-run-length.md) of the processed prefix. A false entry resets the length to zero; a true entry extends it by one.
```
val rowCount = Array.ofDim[Int](N, N)
var i = 0
while (i < N) {
  var j = 0
  var run = 0
  while (j < N) {
    if (a(i)(j)) run += 1 else run = 0
    rowCount(i)(j) = run
    j += 1
  }
  i += 1
}
```
The outer [loop invariant](../../../../../loop-invariant.md) states that rows before `i` have all their correct [row run lengths](../../../../../row-run-length.md). The inner [loop invariant](../../../../../loop-invariant.md) states that columns before `j` in row `i` are correct and that `run` is the length of the all-true suffix of `a(i)[0..j)`. Initially this suffix is empty. Updating `run` gives exactly the suffix length ending at column `j`, proving the required formula, including zero at a false entry. Every cell is visited once:

$$
\boxed{\mathrm{rowCount}(i)(j)=\begin{cases}0,&\neg a(i)(j),\\1+\mathrm{rowCount}(i)(j-1),&a(i)(j),\end{cases}\qquad O(N^2),}
$$

where the fictitious value at column $-1$ is zero. The table itself uses $O(N^2)$ storage.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
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
