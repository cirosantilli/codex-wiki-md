# Lower bounds on network flow

↑ **Parent:** [Flow network](flow-network-split.md)

A prescribed minimum amount on each directed [edge](edge-of-a-graph.md) can be removed by substituting $f_e=\ell_e+x_e$. The new [capacity constraints](capacity-constraint.md) are $0\leq x_e\leq c_e-\ell_e$. For a [circulation with vertex demands](circulation-with-vertex-demands.md) using net inflow $d_v$, the adjusted demand is $d'_v=d_v-(\sum_u\ell_{uv}-\sum_w\ell_{vw})$. Solving the adjusted problem and adding $\ell$ back gives a one-to-one correspondence of [feasible solutions](feasible-point.md). In particular, removing a lower bound on $u\to v$ increases $u$'s residual demand and decreases $v$'s by that amount.

## ↑ Ancestors (6)

1. [Flow network](flow-network-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms/2/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms/2/c/solution.md)
