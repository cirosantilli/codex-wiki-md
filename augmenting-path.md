# Augmenting path

↑ **Parent:** [Residual network](residual-network.md)

An [augmenting path](augmenting-path.md) is a source-to-sink [graph path](path-in-a-graph.md) $P$ of positive capacities in the [residual network](residual-network.md). Its bottleneck is $\Delta=\min_{e\in P}c_f(e)>0$. Add $\Delta$ to original [flow](flow.md) on forward residual [edges](edge-of-a-graph.md) and subtract $\Delta$ on backward residual [edges](edge-of-a-graph.md). Each internal [vertex](vertex-graph-theory.md) still satisfies [flow conservation](flow-conservation.md), and the bottleneck guarantees every [capacity constraint](capacity-constraint.md). The resulting [feasible flow](feasible-flow.md) has [strength of a flow](strength-of-a-flow.md) $|f|+\Delta$. In the unit-capacity [residual network](residual-network.md) example, $\Delta=1$, and the subtraction on $a\to b$ is precisely what allows the value to rise from $1$ to $2$.

**Table of contents**

- [Widest augmenting path](widest-augmenting-path.md)
  - [Geometric convergence of widest-path augmentation](geometric-convergence-of-widest-path-augmentation.md)
- [Ford-Fulkerson algorithm](ford-fulkerson-algorithm.md)
  - [Integrality of the Ford-Fulkerson algorithm](integrality-of-the-ford-fulkerson-algorithm.md)

## ↑ Ancestors (8)

1. [Residual network](residual-network.md)
2. [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
3. [Flow network](flow-network.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Augmenting path](augmenting-path.md)
- [Ford-Fulkerson algorithm](ford-fulkerson-algorithm.md)
- [Maximum flow problem](maximum-flow-problem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4/20d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/c/solution.md)
- [Residual network](residual-network.md)
- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
- [Widest augmenting path](widest-augmenting-path.md)
