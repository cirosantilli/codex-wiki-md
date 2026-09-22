# Generalized pigeonhole principle

↑ **Parent:** [Pigeonhole principle](pigeonhole-principle.md)

For $N$ objects assigned to $m\geq1$ boxes, let $n_i$ be the number in box $i$. The [generalized pigeonhole principle](generalized-pigeonhole-principle.md) states

$$
n_1+\cdots+n_m=N
\quad\Longrightarrow\quad
\max_{1\leq i\leq m}n_i\geq\left\lceil\frac Nm\right\rceil.
$$

The [ceiling function](ceiling-function.md) rounds up because box counts are [integers](integer.md). An equivalent threshold formulation says: for a [positive integer](positive-integer.md) $k$, if $N>m(k-1)$, some box contains at least $k$ objects. For $N=m(k-1)$, putting $k-1$ objects in each box shows why the strict inequality matters. [Lehman, Leighton and Meyer, Mathematics for Computer Science, section 14.8.1, rule 14.8.2](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/mit6_042js15_textbook.pdf#page=583)

**Computed examples.** For $N=13$ and $m=12$, $\lceil13/12\rceil=2$. Counts $(2,1,1,1,1,1,1,1,1,1,1,1)$ attain this bound. For $N=23$ and $m=7$, $\lceil23/7\rceil=4$, and the balanced counts $(4,4,3,3,3,3,3)$ sum to $23$ and have largest count exactly $4$. The threshold version agrees: $23>7(4-1)=21$. In contrast, seven boxes each containing three hold only $21$ objects.

<a id="image-two-balanced-arrangements-attain-the-generalized-pigeonhole-principle-bounds-thirteen-objects-in-twelve-boxes-force-two-and-twenty-three-in-seven-force-four"></a>
![](pigeonhole-distribution-counts.png)

**[Figure 2](#image-two-balanced-arrangements-attain-the-generalized-pigeonhole-principle-bounds-thirteen-objects-in-twelve-boxes-force-two-and-twenty-three-in-seven-force-four). Two balanced arrangements attain the generalized pigeonhole principle bounds: thirteen objects in twelve boxes force two, and twenty-three in seven force four**.

The bound is sharp for every $N$ and $m$. Use [Euclidean division](euclidean-division.md) to write $N=qm+r$ with [integers](integer.md) $q\geq0$ and $0\leq r<m$. Place $q+1$ objects in each of $r$ boxes and $q$ objects in each remaining box. The largest count is $q+1$ if $r>0$, and $q$ if $r=0$, exactly $\lceil N/m\rceil$. This balanced arrangement makes the guarantee best possible even though other arrangements can be much more crowded.

**Proof outline.** If every count were at most $k-1$, the total would be at most $m(k-1)$. This contradicts $N>m(k-1)$. Taking $k=\lceil N/m\rceil$ proves the displayed bound for $N>0$; for $N=0$ every count is zero.

## ↑ Ancestors (5)

1. [Pigeonhole principle](pigeonhole-principle.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Generalized pigeonhole principle](generalized-pigeonhole-principle.md)
- [Pigeonhole principle](pigeonhole-principle.md)
