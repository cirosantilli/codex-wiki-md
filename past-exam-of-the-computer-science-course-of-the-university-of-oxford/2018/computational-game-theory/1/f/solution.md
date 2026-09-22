<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Continue with $0<h<d$ and set $r=d/h$. Part (e) requires an interior count to satisfy $s\leq r\leq s+1$ with $s\geq k$; the all-deer endpoint $s=n$ is allowed when $r\geq n$. If $r$ is nonintegral and $k\leq r<n$, only $s=\lfloor r\rfloor$ works. If $r=m$ is an integer with $k+1\leq m\leq n$, both $s=m-1$ and $s=m$ work. At $r=k$ only $s=k$ remains, while $r>n$ permits only $s=n$. When $r<k$, there is no positive equilibrium count.

Thus there are **at most two positive counts**, and **exactly one** precisely when

$$
\boxed{\frac dh\geq k\quad\text{and}\quad\frac dh\notin\{k+1,k+2,\ldots,n\}.}
$$

This includes $k=n$, when the excluded set is empty. It counts numbers of deer hunters, not the many choices of which hunters participate. The argument is the [threshold stag-hunt equilibrium count](../../../../../threshold-stag-hunt-equilibrium-count.md).

The original paper states only $h<d$ explicitly. Its assertion needs the usual strict positivity of the hare reward. If zero is included, take $n=6,k=4,d=1,h=0$. Counts $s=1$ and $s=2$ both give unsuccessful hunters zero, and one additional deer hunter still cannot reach the threshold; all unilateral alternatives also pay zero. The count $s=6$ is an equilibrium as well. These are **three positive equilibrium counts**, contradicting an unrestricted reading. More generally, for $h=0<d$, the positive counts are $1,\ldots,k-2$ and $n$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
