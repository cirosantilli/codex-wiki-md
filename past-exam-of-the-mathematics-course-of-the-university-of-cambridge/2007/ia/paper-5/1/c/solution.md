<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume head comparison and construction of one list cell take constant time. In the [merge algorithm](../../../../../../merge-algorithm.md), every comparison removes one head from the recursive inputs, and evaluation stops as soon as either is empty. For lengths $m,n>0$, at most $m+n-1$ comparisons and the same number of newly constructed cells are required; the untouched suffix is shared. Inputs which keep both lists nonempty until the last comparison attain this bound. Thus

$$
\boxed{T_{\rm merge}(m,n)=O(m+n),\quad\text{with worst case }\Theta(m+n).}
$$

An initially empty input makes this particular implementation constant-time; not every pair requires linear work.

The balanced [merge sort](../../../../../../merge-sort.md) spends $\Theta(n)$ time per call on list length, splitting and merging. Hence its [time complexity](../../../../../../time-complexity.md) satisfies

$$
T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+\Theta(n),\qquad T(0),T(1)=\Theta(1).
$$

At each recursion level the lengths of its disjoint subproblems sum to $n$, so the work per level is $\Theta(n)$, and balanced splitting gives $\Theta(\log n)$ levels. Consequently

$$
\boxed{T_{\rm mergesort}(n)=\Theta(n\log n)\quad(n\ge2).}
$$

The length and splitting traversals change the constant factor, not this asymptotic order; repeatedly inserting elements into a sorted list would not give the same complexity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
