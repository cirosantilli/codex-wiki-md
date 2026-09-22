# Directed acyclic graph

↑ **Parent:** [Combinatorics](combinatorics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Directed_acyclic_graph)

A [Directed acyclic graph](directed-acyclic-graph.md) is a [directed graph](directed-graph.md) with no [directed cycle](directed-cycle.md): following its [directed edges](directed-edge.md) can never return to the starting [vertex](vertex-graph-theory.md). A [directed edge](directed-edge.md) $u\to v$ can represent the requirement that task $u$ finish before task $v$ starts. A [directed path](directed-path.md) then records a chain of prerequisites. The essential prerequisite for [topological sorting](topological-sorting.md) is that these requirements contain no circular dependency. For finite [directed graphs](directed-graph.md), this is equivalent to the existence of a [topological order](topological-order.md). [MIT, Introduction to Algorithms, Recitation 10, p. 3: directed acyclic graphs and topological sorts](https://live.ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/d9265b3b33d238ff914b0223ac8e7628_MIT6_006S20_r10.pdf)

Consider an invented publishing workflow with five tasks: $A$ drafts the text, $B$ draws a figure, $C$ reviews the text, $D$ lays out the text and figure, and $E$ publishes the result. Its [directed edges](directed-edge.md) are $A\to C$, $A\to D$, $B\to D$, $C\to E$, and $D\to E$. Reviewing needs the draft; layout needs both the draft and figure; publication needs both review and layout. The drawing below encodes only these prerequisites, with no measured durations or resource constraints.

<a id="image-five-toy-publishing-tasks-and-all-five-valid-topological-orders"></a>
![](topological-task-dependency-orders.png)

**[Figure 9](#image-five-toy-publishing-tasks-and-all-five-valid-topological-orders). Five toy publishing tasks and all five valid topological orders**.

The [Directed acyclic graph](directed-acyclic-graph.md) leaves room for choice: $A$ and $B$ can occur in either order, and after both are complete, $C$ and $D$ can occur in either order. Task $C$ may even precede $B$, since the review does not need the figure. A [topological order](topological-order.md) turns these local prerequisites into a complete executable list while retaining this freedom. It supplies a feasible sequential plan; task durations, available workers, and earliest finishing times require additional information.

**Table of contents**

- [Topological sorting](topological-sorting.md)
  - [Topological order](topological-order.md)
  - [Kahn's algorithm](kahn-s-algorithm.md)
- [Markov equivalence of directed acyclic graphs](markov-equivalence-of-directed-acyclic-graphs.md)
  - [Completed partially directed acyclic graph](completed-partially-directed-acyclic-graph.md)
  - [Skeleton and collider characterization of Markov equivalence](skeleton-and-collider-characterization-of-markov-equivalence.md)
- [Moral graph](moral-graph.md)
  - [Hammersley-Clifford theorem](hammersley-clifford-theorem.md)
- [Topological ordering](topological-ordering.md)
- [D-separation](d-separation.md)
  - [Collider](collider.md)
    - [Unshielded collider](unshielded-collider.md)
  - [D-separating set](d-separating-set.md)
  - [Local Markov property of a directed acyclic graph](local-markov-property-of-a-directed-acyclic-graph.md)
  - [Global Markov property of a directed acyclic graph](global-markov-property-of-a-directed-acyclic-graph.md)

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (45)

- [Acyclic orientation](acyclic-orientation.md)
- [Arithmetic circuit](arithmetic-circuit.md)
- [Bayesian network](bayesian-network.md)
- [Causal minimality](causal-minimality.md)
- [Critical path method](critical-path-method.md)
- [Directed acyclic graph](directed-acyclic-graph.md)
- [Directed acyclic graph factorization](directed-acyclic-graph-factorization.md)
- [Dynamic programming](dynamic-programming.md)
- [Faithfulness of a directed acyclic graph](faithfulness-of-a-directed-acyclic-graph.md)
- [Global Markov property for a directed acyclic graph](global-markov-property-for-a-directed-acyclic-graph.md)
- [Global Markov property of a directed acyclic graph](global-markov-property-of-a-directed-acyclic-graph.md)
- [Indegree](indegree.md)
- [Markov blanket](markov-blanket.md)
- [Markov blanket D-separation](markov-blanket-d-separation.md)
- [Markov equivalence of directed acyclic graphs](markov-equivalence-of-directed-acyclic-graphs.md)
- [Memoization](memoization.md)
- [Memoized Fibonacci evaluation](memoized-fibonacci-evaluation.md)
- [Moral graph](moral-graph.md)
- [Moral graph equals the conditional independence graph under faithfulness](moral-graph-equals-the-conditional-independence-graph-under-faithfulness.md)
- [Order-induced acyclic orientation](order-induced-acyclic-orientation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-39/3/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-59/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/2/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-207/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-207/1/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-221/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-219/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-221/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-221/2/iii/solution.md)
- [PC initialization from a conditional independence graph](pc-initialization-from-a-conditional-independence-graph.md)
- [Pedigree graphical model](pedigree-graphical-model.md)
- [Project scheduling](project-scheduling.md)
- [Skeleton and collider characterization of Markov equivalence](skeleton-and-collider-characterization-of-markov-equivalence.md)
- [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
- [Task float](task-float.md)
- [Topological order](topological-order.md)
- [Topological ordering](topological-ordering.md)
- [Topological sorting](topological-sorting.md)
- [Unshielded collider](unshielded-collider.md)
