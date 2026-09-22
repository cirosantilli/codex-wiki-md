# Adjacency-matrix bound for a discrete SIR epidemic

↑ **Parent:** [Discrete SIR epidemic on a graph](discrete-sir-epidemic-on-a-graph.md)

The conditional [union bound](boole-s-inequality.md) gives $\mathbb EX_i(k+1)\leq\beta\sum_jA_{ij}\mathbb EX_j(k)$ in a [discrete SIR epidemic on a graph](discrete-sir-epidemic-on-a-graph.md). Iteration bounds the infection vector at step $k$ by $(\beta A)^kX(0)$. Each [vertex](vertex-graph-theory.md) is infected at most once, so summing the probabilities in time gives the displayed bound. Powers of the [adjacency matrix of a graph](adjacency-matrix.md) count [walks](walk-in-a-graph.md), which can overcount impossible reinfections without invalidating the upper bound. Initially removed individuals must be counted separately when bounding all eventual removals.

**Table of contents**

- [Resolvent bound for a discrete SIR epidemic](resolvent-bound-for-a-discrete-sir-epidemic.md)
  - [Spectral condition for a small discrete SIR outbreak](spectral-condition-for-a-small-discrete-sir-outbreak.md)

## ↑ Ancestors (7)

1. [Discrete SIR epidemic on a graph](discrete-sir-epidemic-on-a-graph.md)
2. [SIR model](sir-model.md)
3. [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)
4. [Mathematical biology](mathematical-biology-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-36/4/a/solution.md)
- [Resolvent bound for a discrete SIR epidemic](resolvent-bound-for-a-discrete-sir-epidemic.md)
