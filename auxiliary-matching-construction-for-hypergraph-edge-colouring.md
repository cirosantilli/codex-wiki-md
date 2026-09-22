# Auxiliary matching construction for hypergraph edge colouring

↑ **Parent:** [Hypergraph chromatic index](hypergraph-chromatic-index.md)

Given an $r$-uniform [hypergraph](hypergraph-split.md) $H$ and $K$ colours, construct an $(r+1)$-uniform auxiliary [hypergraph](hypergraph-split.md) with one task vertex for every $e\in E(H)$ and one resource vertex $(v,c)$ for every original vertex and colour. The assignment edge for $(e,c)$ contains the task $e$ and all resources $(v,c)$ with $v\in e$. A [matching in a hypergraph](matching-in-a-hypergraph.md) of assignments is exactly a proper partial edge colouring. Task degrees are $K$; resource degrees are $d_H(v)$. Pairwise auxiliary [hypergraph codegrees](hypergraph-codegree.md) are at most $\max(1,\max_{v\ne w}d_H(v,w))$. Thus nearly equal original degrees and small original [hypergraph codegrees](hypergraph-codegree.md) transfer to the setting of a [Rödl nibble](rodl-nibble.md). A locally balanced [Rödl nibble](rodl-nibble.md) must control the unmatched task count in every original star, not merely the total uncovered proportion.

## ↑ Ancestors (8)

1. [Hypergraph chromatic index](hypergraph-chromatic-index.md)
2. [Hypergraph colouring](hypergraph-colouring.md)
3. [Hypergraph](hypergraph-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/4/solution.md)
