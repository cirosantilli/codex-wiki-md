# Cycle lemma

↑ **Parent:** [Combinatorics](combinatorics-split.md)

The [cycle lemma](cycle-lemma.md) turns a constraint at every prefix into a choice of where to start reading a circular [sequence](sequence.md). Think of a [lattice path](lattice-path.md) whose vertical increments record votes for two candidates: $+1$ for one candidate and $-1$ for the other. Its [partial sums](partial-sum.md) are the running lead. Rotating the increments preserves the final lead, but changes whether that lead stays strictly positive throughout. This makes rotation useful for counting [lattice paths](lattice-path.md) subject to prefix constraints; the sum-one [cycle lemma](cycle-lemma.md) also supplies the cyclic prefix condition in the [cyclic Turán covering construction](cyclic-turan-covering-construction.md).

**The sum-one form.** Let $b=(b_1,\ldots,b_n)$ be any nonempty [sequence](sequence.md) of [integers](integer.md) with $\sum_{i=1}^n b_i=1$. A starting position $r\in\{0,\ldots,n-1\}$ means reading the rotated [sequence](sequence.md)

$$
b^{(r)}=(b_{r+1},\ldots,b_n,b_1,\ldots,b_r).
$$

Call $r$ good when every nonempty [partial sum](partial-sum.md) of $b^{(r)}$ is strictly positive, including the full [sum](sum.md):

$$
P_j^{(r)}=\sum_{i=1}^{j}b_i^{(r)}>0\qquad(1\leq j\leq n).
$$

The [cycle lemma](cycle-lemma.md) says there is exactly one good starting position. Negative entries, zero entries and positive entries larger than one are all allowed in this sum-one form. The empty [partial sum](partial-sum.md) is zero and is excluded from the positivity requirement. Douglas West's exercise 1.3.46(a) states a stronger result for arbitrary [integer](integer.md) entries: take its case with all $n$ [partial sums](partial-sum.md) positive. [West, Combinatorial Mathematics, exercise 1.3.46(a), p. 50](https://api.pageplace.de/preview/DT0400.9781108889520_A49236431/preview-9781108889520_A49236431.pdf#page=72)

**A worked sum-one example.** For $b=(2,-2,0,1)$, the [partial sums](partial-sum.md) starting at zero are $S_0,S_1,S_2,S_3,S_4=0,2,0,0,1$. Starts $0,1,2$ fail: they have, respectively, a zero second [partial sum](partial-sum.md), a negative first [partial sum](partial-sum.md), and a zero first [partial sum](partial-sum.md). Start $3$ reads $(1,2,-2,0)$ and has nonempty [partial sums](partial-sum.md) $1,3,1,1$, all positive. This example both allows an increment larger than one and shows why touching zero fails.

**Why the last minimum works.** Put $S_0=0$ and $S_j=\sum_{i=1}^j b_i$. Choose the last index $r$ attaining the [minimum](minimum-of-a-subset-of-a-total-order.md) of the proper [partial sums](partial-sum.md) $S_0,\ldots,S_{n-1}$: include $S_0$ and exclude $S_n$. After that index, later proper [partial sums](partial-sum.md) are strictly larger than $S_r$; also $S_n=1>S_r$, since $S_r\leq0$. Before wrapping, the new [partial sums](partial-sum.md) are therefore positive differences $S_j-S_r$. After wrapping, they are $1+S_j-S_r\geq1$. In the worked example the last [minimum](minimum-of-a-subset-of-a-total-order.md) is at $r=3$; choosing the first [minimum](minimum-of-a-subset-of-a-total-order.md) at $r=0$ would fail. Uniqueness takes one further observation: two good starts would split the circle into two nonempty arcs, each having a positive [integer](integer.md) [sum](sum.md), yet their [sum](sum.md) would be one.

**Table of contents**

- [Cycle lemma with increments at most one](cycle-lemma-with-increments-at-most-one.md)

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Cycle lemma](cycle-lemma.md)
- [Cycle lemma with increments at most one](cycle-lemma-with-increments-at-most-one.md)
- [Cyclic Turán covering construction](cyclic-turan-covering-construction.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110/5/solution.md)
