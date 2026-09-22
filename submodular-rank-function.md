# Submodular rank function

↑ **Parent:** [Rank of a matroid](rank-of-a-matroid.md)

On a finite [ground set](ground-set.md) $E$, a submodular rank function is a [normalised set function](normalised-set-function.md) $r$ with $r(\varnothing)=0$, a [monotone set function](monotone-set-function.md), and a [submodular set function](submodular-set-function.md), such that $r(A\cup\{e\})-r(A)\in\{0,1\}$ for $e\notin A$. Equivalently, require nonnegative [integer](integer-split.md) values, monotonicity, [submodularity](submodular-set-function.md) and $r(\{e\})\leq1$. The [diminishing returns characterization of submodularity](diminishing-returns-characterization-of-submodularity.md) bounds each marginal by its [singleton](singleton-mathematics.md) value. Thus $0\leq r(A)\leq|A|$.

These functions are precisely the [rank functions of matroids](rank-of-a-matroid.md). To see the converse direction, define $\mathcal I=\{A:r(A)=|A|\}$. It contains the empty set. If $B\subseteq A\in\mathcal I$, the unit marginal bounds give $|A|=r(A)\leq r(B)+|A\setminus B|$, so $r(B)=|B|$ and heredity holds. For augmentation, suppose $A,B\in\mathcal I$ with $|A|<|B|$. If every $e\in B\setminus A$ had zero marginal over $A$, diminishing returns would keep each marginal zero as they are added successively. This would give $r(A\cup B)=r(A)=|A|<|B|=r(B)$, contradicting monotonicity. Some marginal is therefore one, giving an independent augmentation.

Finally any inclusion-maximal $I\subseteq A$ in this independence family has $r(I\cup\{e\})=r(I)$ for every remaining $e\in A\setminus I$. Successively adding them and using diminishing returns shows $r(A)=r(I)=|I|$, so the resulting [matroid](matroid.md) really has rank $r$. The forward direction is [submodularity of matroid rank](submodularity-of-matroid-rank.md). These [integer](integer-split.md) increment conditions distinguish [matroid](matroid.md) ranks from arbitrary real-valued submodular functions.

## ↑ Ancestors (6)

1. [Rank of a matroid](rank-of-a-matroid.md)
2. [Matroid](matroid.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2011/1/c/solution.md)
