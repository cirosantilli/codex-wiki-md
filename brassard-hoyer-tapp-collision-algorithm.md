<h1 id="brassard-hoyer-tapp-collision-algorithm">Brassard–Høyer–Tapp collision algorithm</h1>

↑ **Parent:** [Quantum collision finding](quantum-collision-finding.md)

Query a known set of $m$ inputs and store its output table. If no [function collision](function-collision.md) occurs there, each of its $m$ distinct outputs has exactly one partner in the complement, for a two-to-one function. A [compute-phase-uncompute construction](compute-phase-uncompute-construction.md) marks those partners using two function queries and reversible table comparison. [Known-subset Grover search](known-subset-grover-search.md) then uses $O(\sqrt{(N-m)/m})$ such phase queries. Including table preparation and a final verification query gives

$$
T(m)=m+O\!\left(\sqrt{\frac{N-m}{m}}\right)+1.
$$

Choosing $m\asymp N^{1/3}$ balances both terms and gives $T(m)=O(N^{1/3})$. The [Grover rotation angle](grover-rotation-angle.md) rounding bound gives success tending to one. This is a query bound; it does not make reversible table lookup free in a gate or physical-memory cost model.

## ↑ Ancestors (7)

1. [Quantum collision finding](quantum-collision-finding.md)
2. [Quantum query complexity](quantum-query-complexity.md)
3. [Quantum complexity theory](quantum-complexity-theory.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/2/b/solution.md)
