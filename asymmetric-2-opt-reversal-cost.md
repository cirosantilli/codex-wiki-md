# Asymmetric 2-opt reversal cost

↑ **Parent:** [2-opt](2-opt.md)

A 2-opt schedule move reverses a consecutive block $v_p,\ldots,v_q$, reconnecting its boundary arcs. With directed costs, its change is

$$
\Delta=c_{v_{p-1},v_q}+c_{v_p,v_{q+1}}
-c_{v_{p-1},v_p}-c_{v_q,v_{q+1}}
+\sum_{r=p}^{q-1}(c_{v_{r+1},v_r}-c_{v_r,v_{r+1}}).
$$

Omitting the internal sum is valid only for symmetric costs. A [simulated annealing](simulated-annealing.md) step accepts an increase with probability $\exp(-\Delta/T)$; a strictly positive temperature permits escape from local minima.

## ↑ Ancestors (6)

1. [2-opt](2-opt.md)
2. [Travelling salesman problem](travelling-salesman-problem.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [2-opt](2-opt.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/5/b/solution.md)
