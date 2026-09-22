<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $s_j$ be the total length of the two runs in merge $j$. Because destinations are always appended beyond the old endpoint, the exact space consumption is

$$
d=n+\sum_j s_j.
$$

A simple valid bound is $d\leq n+n(n-1)=n^2$, using at most $n-1$ merges. The [FIFO queue](../../../../../fifo-queue.md) schedule permits the sharper asymptotic bound

$$
\boxed{d=\Theta(n\log n)\text{ in the worst case for }n\geq2.}
$$

To prove the upper bound, group merges into rounds. Mark the old end of the live segment, and finish a round when all runs present at its start have been consumed. If there are $R>1$ such runs, at most $\lceil R/2\rceil$ merges occur. Only the last merge can pair one remaining old run with an already appended run. Consequently at most $\lceil R/2\rceil$ runs remain; coalescence can only reduce this number. Every start-of-round entry is merged once, and entries in the one possible already appended run are merged at most once more. A round writes at most $2n$ entries. After at most $\lceil\log_2 R_0\rceil$ rounds there is one run, giving $d\leq n+2n\lceil\log_2 R_0\rceil$ for $R_0\geq2$.

For a matching family, let $n=2^{h+1}$ and use $2^h$ repetitions of $[0,1]$. Each initial run has length two. Every merged run still starts at zero and ends at one, so adjacent runs never coalesce. In each of the $h$ complete merging levels exactly $n$ entries are written. Hence

$$
d=n+nh=n\log_2 n
$$

on this family. For an already sorted input, no merge occurs and $d=n$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
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
