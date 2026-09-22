# Closure of a matroid

↑ **Parent:** [Matroid](matroid.md)

The [closure of a matroid](closure-of-a-matroid.md) adds all elements that fail to increase its [rank of a matroid](rank-of-a-matroid.md). It abstracts the [linear span](linear-span.md) in a [linear matroid](linear-matroid.md). It is extensive, preserves inclusion, preserves the [rank of a matroid](rank-of-a-matroid.md), and is an [idempotent function](idempotent-function.md):

$$
A\subseteq\operatorname{cl}_M(A),\qquad
A\subseteq B\Rightarrow\operatorname{cl}_M(A)\subseteq\operatorname{cl}_M(B),\qquad
r(\operatorname{cl}_M(A))=r(A),\qquad
\operatorname{cl}_M(\operatorname{cl}_M(A))=\operatorname{cl}_M(A).
$$

**Proof.** Extensivity follows from $A+x=A$ when $x\in A$. If $A\subseteq B$ and $x\notin B$, [submodularity of matroid rank](submodularity-of-matroid-rank.md) gives $r(B+x)-r(B)\leq r(A+x)-r(A)$. Thus an element in $\operatorname{cl}_M(A)$ also lies in $\operatorname{cl}_M(B)$; the case $x\in B$ is automatic. Add the finitely many elements of $\operatorname{cl}_M(A)\setminus A$ one at a time. Inclusion preservation makes each addition have zero [marginal increment](marginal-increment-of-a-set-function.md) of the [rank of a matroid](rank-of-a-matroid.md), proving rank preservation.

For completeness, nested [subsets](subset.md) $A\subseteq B$ of equal [rank of a matroid](rank-of-a-matroid.md) have the same [closure of a matroid](closure-of-a-matroid.md). If $x\notin B$, apply [submodularity of matroid rank](submodularity-of-matroid-rank.md) to $B$ and $A+x$ to obtain $r(B+x)\leq r(A+x)$; monotonicity gives the reverse bound. The defining tests for membership in their closures are therefore equal. If $x\in B$, $r(A)\leq r(A+x)\leq r(B)=r(A)$, so both closures contain $x$. Apply this equal-rank result to $A\subseteq\operatorname{cl}_M(A)$ to prove idempotence. In particular, every maximal [matroid independent set](independent-set-of-a-matroid.md) of $B$ has the same [closure of a matroid](closure-of-a-matroid.md) as $B$.

## ↑ Ancestors (5)

1. [Matroid](matroid.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Closure of a matroid](closure-of-a-matroid.md)
- [Loop of a matroid](loop-of-a-matroid.md)
- [Matroid closure exchange property](matroid-closure-exchange-property.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/2/c/ii/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/2/c/iv/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/2/c/v/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/2/c/vi/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/2/c/vii/solution.md)
