# Bounded-size transversal kernel

↑ **Parent:** [Hitting set](hitting-set.md)

If the members of a possibly infinite [set family](set-family.md) $\mathcal F$ have size at most $r$, there is a finite [subset](subset.md) $\mathcal F_0\subseteq\mathcal F$ of size at most $M(r,s)$ with exactly the same [hitting sets](hitting-set.md) of size at most $s$. Use [mathematical induction](mathematical-induction.md) on $s$. For nonempty $\mathcal F$, choose $A_0\in\mathcal F$. When $s=0$ this one member suffices. Otherwise, for each $x\in A_0$, retain an inductive kernel for $\mathcal F_x=\{A\in\mathcal F:x\notin A\}$ at parameter $s-1$, and take their [set union](set-union.md) together with $A_0$. Its size is at most $1+rM(r,s-1)=M(r,s)$. A [hitting set](hitting-set.md) $H$ for this kernel meets $A_0$ at some $x$; $H\setminus\{x\}$ meets the kernel for $\mathcal F_x$, hence all of $\mathcal F_x$, while $x$ meets the other members of $\mathcal F$. If $A_0$ is empty no [hitting set](hitting-set.md) exists, and if $\mathcal F$ is empty its kernel is empty. Only finite branching is used, so no finiteness assumption on $\mathcal F$ is needed.

## ↑ Ancestors (7)

1. [Hitting set](hitting-set.md)
2. [Set family](set-family.md)
3. [Extremal set theory](extremal-set-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite intersection witness for cross-intersecting families](finite-intersection-witness-for-cross-intersecting-families.md)
- [Hitting set](hitting-set.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-109/2/ii/solution.md)
