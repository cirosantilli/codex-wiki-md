# Colour-focusing proof of Van der Waerden theorem

↑ **Parent:** [Van der Waerden theorem](van-der-waerden-theorem.md)

For positive $r,k$, let $W(r,k)$ bound the interval needed to force a [monochromatic](monochromatic-set.md) length-$k$ [arithmetic progression](arithmetic-progression.md) in every [finite colouring](finite-coloring.md) using at most $r$ colours. The [colour-focusing proof of Van der Waerden theorem](colour-focusing-proof-of-van-der-waerden-theorem.md) inducts on $k$, simultaneously for every number of colours, and then creates progressions of distinct colours with a common next point.

Assume $W(r,k)$ exists for every $r$. For fixed $r$, construct $F_t$ such that a [finite colouring](finite-coloring.md) of $[F_t]$ using at most $r$ colours contains either a [monochromatic](monochromatic-set.md) length-$(k+1)$ [arithmetic progression](arithmetic-progression.md), or $t$ length-$k$ [arithmetic progressions](arithmetic-progression.md) of pairwise distinct colours of the form $f-hd_i$, $1\le h\le k$, with a common focus $f\in[F_t]$. Take $F_1=2W(r,k)$: a length-$k$ [arithmetic progression](arithmetic-progression.md) in its first half has its next point inside the whole interval. For $k=1$, give a singleton step $1$.

Given $N=F_t$, put $M=W(r^N,k)$ and $F_{t+1}=2NM$. Regard the first $M$ length-$N$ blocks as coloured by their full [colour profiles](colour-profile-of-a-finite-block.md). Some block indices $j_0,j_0+D,\ldots,j_0+(k-1)D$ share a profile. If there is no [monochromatic](monochromatic-set.md) length-$(k+1)$ [arithmetic progression](arithmetic-progression.md), this profile supplies $t$ focused progressions with focus position $f$, steps $d_i$, and distinct colours $q_i$. The colour $q$ of position $f$ differs from every $q_i$. In the later block $j_*=j_0+kD\le2M$, put $F=N(j_*-1)+f$. For each $i$, the points $F-h(ND+d_i)$ have colour $q_i$: they lie in the selected block $j_*-hD$ at position $f-hd_i$. The points $F-hND$ have colour $q$. Thus $t+1$ distinct colours focus at $F$. For $t=r$, its own colour completes one of the $r$ focused progressions. The base case $W(r,1)=1$ completes the [mathematical induction](mathematical-induction.md).

## ↑ Ancestors (6)

1. [Van der Waerden theorem](van-der-waerden-theorem.md)
2. [Ramsey theory](ramsey-theory-split.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Colour-focusing proof of Van der Waerden theorem](colour-focusing-proof-of-van-der-waerden-theorem.md)
- [Colour profile of a finite block](colour-profile-of-a-finite-block.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-10/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14/2/solution.md)
