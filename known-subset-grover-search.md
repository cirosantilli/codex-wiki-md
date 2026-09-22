# Known-subset Grover search

↑ **Parent:** [Grover's algorithm](grover-s-algorithm.md)

For a known finite set $B$, prepare the [uniform superposition state](uniform-superposition-state.md) $|s_B\rangle$ and implement its [reflection operator](reflection-operator.md) $2|s_B\rangle\langle s_B|-I$. If exactly $k$ basis states in $B$ are marked, the same two-dimensional [Grover rotation angle](grover-rotation-angle.md) argument uses $O(\sqrt{|B|/k})$ phase queries. Preparation and reflection are known operations with no calls to the unknown predicate. Their gate cost must be accounted for separately. The success guarantee requires $k>0$, and choosing the optimal iteration number uses a known $k$.

**Table of contents**

- [Clean subset superposition preparation](clean-subset-superposition-preparation.md)

## ↑ Ancestors (5)

1. [Grover's algorithm](grover-s-algorithm.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Brassard–Høyer–Tapp collision algorithm](brassard-hoyer-tapp-collision-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/2/b/solution.md)
