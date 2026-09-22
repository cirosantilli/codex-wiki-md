<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use binary units $1\mathrm{KB}=2^{10}$ bytes and $1\mathrm{MB}=2^{20}$ bytes, consistent with the given binary GB convention. Reading one average file takes seek plus rotation plus transfer; moving it requires the same costs again on the write:

$$
\boxed{t_{\rm file}=2\left(0.005+0.004+\frac{8\cdot2^{10}}{8\cdot2^{20}}\right)=0.019953125\text{ s}\approx20\text{ ms}.}
$$

A half-full 16 GB disk contains $8\cdot2^{30}$ used bytes, or $N=2^{20}$ average files. Under the stated per-file [disk compaction](../../../../../disk-compaction.md) model,

$$
\boxed{T=N t_{\rm file}=20922.368\text{ s}\approx5.81\text{ hours}.}
$$

A calculation with decimal KB and MB changes the unrounded figures, so the unit convention must be retained consistently. This model charges one seek and rotational delay on each read and each write; it does not assume a single streaming pass over the whole disk.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
