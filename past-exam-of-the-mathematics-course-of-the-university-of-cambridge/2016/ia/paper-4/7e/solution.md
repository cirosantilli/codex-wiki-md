<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

For finite sets $E_1,\ldots,E_s$, the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) states

$$
\left|\bigcup_{j=1}^s E_j\right|
=\sum_{\varnothing\ne I\subseteq\{1,\ldots,s\}}
(-1)^{|I|+1}\left|\bigcap_{j\in I}E_j\right|.
$$

It counts each element once: an element in exactly $q$ of the sets contributes $\sum_{j=1}^q(-1)^{j+1}\binom qj=1$, by the [binomial theorem](../../../../../binomial-theorem.md).

For the [cyclic digit run](../../../../../cyclic-digit-run.md) problem, let $E_j$ mean that the three digits starting at position $j$ form a run, for $j=1,2,3,4$. Every run of length at least three contains one of these triples, so we need $|E_1\cup E_2\cup E_3\cup E_4|$. Introduce the five differences

$$
d_i\equiv a_{i+1}-a_i\pmod{10},\qquad i=1,\ldots,5.
$$

A starting digit and these five residues determine a unique string, including runs that cross $9$ and $0$. In these coordinates $E_j$ requires $(d_j,d_{j+1})=(1,1)$ or $(-1,-1)$.

Each single event fixes two differences, with two choices of sign; the initial digit and the other three differences are free. Thus $|E_j|=10\cdot2\cdot10^3=20000$. For intersections of two events, adjacent starting positions force three consecutive differences to have the same sign, giving $10\cdot2\cdot10^2=2000$. There are three such pairs. The other three pairs have disjoint constrained difference positions, with independent signs and one free difference, giving $10\cdot4\cdot10=400$ each. Consequently the sum of pair-intersection sizes is $3\cdot2000+3\cdot400=7200$.

For triple intersections, $E_1\cap E_2\cap E_3$ and $E_2\cap E_3\cap E_4$ each force four consecutive differences to have the same sign, leaving one free difference, and each has size $10\cdot2\cdot10=200$. The other two triples, $E_1\cap E_2\cap E_4$ and $E_1\cap E_3\cap E_4$, divide the five differences into two blocks with independent signs; each has size $10\cdot4=40$. The triple-intersection sum is therefore $480$. Finally, all four events force all five differences to have the same sign, giving $20$ strings.

The [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) now gives **the number of strings**

$$
\boxed{4\cdot20000-7200+480-20=73260}.
$$

Using differences makes the overlap conditions explicit and prevents double-counting long [cyclic digit runs](../../../../../cyclic-digit-run.md).

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
