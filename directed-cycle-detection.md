# Directed cycle detection

↑ **Parent:** [NL-complete](nl-complete.md)

Decide whether a [directed graph](directed-graph.md) has a nonempty directed cycle; self-loops count. This problem is [NL-complete](nl-complete.md). Membership guesses a returning walk of at most the vertex count. For hardness, layer a reachability instance into $N+1$ layers with wait arcs, then add only the backward edge from the target in the last layer to the source in the first. The otherwise acyclic layering has a cycle exactly when the original target is reachable. Zero-length paths must not be treated as cycles.

## ↑ Ancestors (9)

1. [NL-complete](nl-complete.md)
2. [NL (complexity)](nl-complexity.md)
3. [Logarithmic space](logarithmic-space.md)
4. [Space complexity](space-complexity.md)
5. [Complexity class](complexity-class.md)
6. [Computational complexity theory](computational-complexity-theory.md)
7. [Theoretical computer science](theoretical-computer-science.md)
8. [Computer science](computer-science-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-59/2/b/solution.md)
