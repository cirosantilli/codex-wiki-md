# Critical path method

↑ **Parent:** [Project scheduling](project-scheduling.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Critical_path_method)

Add a dummy source before the initial tasks and a dummy sink after the terminal tasks. Give every arc leaving task $i$ length $\tau_i$, its duration, with zero duration at the source. The longest path length is the minimum possible project duration. Earliest starts are obtained in [topological order](topological-order.md) by $t_j=\max_{i\to j}(t_i+\tau_i)$. A longest path is a critical path.

// Target: mathematical-optimization.bigb

**Table of contents**

- [Project scheduling duality](project-scheduling-duality.md)
  - [Unit-flow certificate for project duration](unit-flow-certificate-for-project-duration.md)

## ↑ Ancestors (5)

1. [Project scheduling](project-scheduling.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/2/solution.md)
