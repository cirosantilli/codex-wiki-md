# Mandatory service dependency

↑ **Parent:** [Distributed system](distributed-system.md)

Fix the operation being considered and the conditions under which it must complete. A [mandatory service dependency](mandatory-service-dependency.md) $u\to v$ means that completing the designated operation of $u$ requires $v$ to supply its designated service. Dependencies can be represented by a [directed graph](directed-graph.md). The operation and conditions matter: an operation that can use an already retained result need not require a new response from its original source.

A [directed path](directed-path.md) of mandatory dependencies propagates necessity. This follows by [mathematical induction](mathematical-induction.md) on the path length: one edge is the definition, and composing one further necessary condition gives the induction step. Consequently, if every replica requires the same component, losing that component can block the operation at every replica. Keeping copies of other components does not remove the shared requirement. Conversely, the availability of every dependency is not by itself a proof that an operation will complete.

## ↑ Ancestors (3)

1. [Distributed system](distributed-system.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Mandatory service dependency](mandatory-service-dependency.md)
- [Solution](past-exam-of-the-internet-technologies-and-regulation-course-of-the-university-of-oxford/2019/1/solution.md)
- [Service availability](service-availability.md)
