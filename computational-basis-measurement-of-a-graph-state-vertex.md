# Computational-basis measurement of a graph-state vertex

↑ **Parent:** [Graph state](graph-state.md)

For a [graph state](graph-state.md) $|G\rangle=\prod_{ij\in E}CZ_{ij}|+\rangle^{\otimes|V|}$, measuring [vertex](vertex-graph-theory.md) $v$ in the [computational basis](computational-basis.md) with result $r$ gives the normalized state

$$
\left(\prod_{u\in N(v)}Z_u^r\right)|G-v\rangle.
$$

Each [Controlled-Z gate](controlled-z-gate.md) from $v$ to a neighbour acts as $Z_u^r$ after projecting $v$ onto $|r\rangle$; all other [edges](edge-of-a-graph.md) remain unchanged. The projection contributes $1/\sqrt2$, so either result has [probability](probability.md) $1/2$. For a four-cycle, deleting one [vertex](vertex-graph-theory.md) leaves a path and adds byproducts on its two endpoints.

## ↑ Ancestors (9)

1. [Graph state](graph-state.md)
2. [Stabilizer state](stabilizer-state.md)
3. [Stabilizer group](stabilizer-group.md)
4. [Pauli group](pauli-group.md)
5. [Quantum circuit](quantum-circuit-split.md)
6. [Quantum theory](quantum-theory-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/4/a/ii/solution.md)
