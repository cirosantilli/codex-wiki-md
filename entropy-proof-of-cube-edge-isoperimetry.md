# Entropy proof of cube edge-isoperimetry

↑ **Parent:** [Edge-isoperimetric inequality in the discrete cube](edge-isoperimetric-inequality-in-the-discrete-cube.md)

For a vertex set of size $m$ in a [hypercube graph](hypercube-graph.md), split one coordinate into sections of sizes $a,b$. Induction bounds the internal edges within the sections by $(a\log_2a+b\log_2b)/2$; at most $\min(a,b)$ edges cross between them. Put $t=\min(a,b)/(a+b)$. The chord bound for the [binary entropy function](binary-entropy-function.md) gives $H_2(t)\ge2t$, hence $a\log_2a+b\log_2b+2\min(a,b)\le m\log_2m$. Thus at most $m\log_2m/2$ internal edges are present, and the [edge boundary](edge-boundary-in-a-graph.md) is at least $m(n-\log_2m)$. Coordinate subcubes attain equality when $m$ is a power of two.

**Table of contents**

- [Equality cases of entropy cube edge-isoperimetry](equality-cases-of-entropy-cube-edge-isoperimetry.md)

## ↑ Ancestors (8)

1. [Edge-isoperimetric inequality in the discrete cube](edge-isoperimetric-inequality-in-the-discrete-cube.md)
2. [Edge boundary in a graph](edge-boundary-in-a-graph.md)
3. [Boolean hypercube](boolean-hypercube.md)
4. [Analysis of Boolean functions](analysis-of-boolean-functions.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-12/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-11/1/i/solution.md)
