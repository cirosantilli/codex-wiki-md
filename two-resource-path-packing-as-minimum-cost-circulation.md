# Two-resource path packing as minimum-cost circulation

↑ **Parent:** [Minimum-cost flow problem](minimum-cost-flow-problem.md)

Consider nonnegative route variables with constraints $u\leq a$, $v\leq b$, $v+w\leq c$, $w+z\leq d$, and a linear reward $p_u u+p_v v+p_w w+p_z z$. It is a [minimum-cost flow](minimum-cost-flow-problem.md) problem: use arcs $s\to t$ of capacity $a$ and cost $-p_u$, $s\to L$ of capacity $c$ and cost zero, $L\to t$ of capacity $b$ and cost $-p_v$, $L\to R$ of unlimited capacity and cost $-p_w$, $s\to R$ of unlimited capacity and cost $-p_z$, and $R\to t$ of capacity $d$ and cost zero. Close the network by an unlimited zero-cost arc $t\to s$. The four forward path flows are exactly $u,v,w,z$, so conservation gives the resource constraints. This reduction does not assert that general multi-commodity flow is ordinary minimum-cost flow.

## ↑ Ancestors (6)

1. [Minimum-cost flow problem](minimum-cost-flow-problem.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/4/solution.md)
