# Blocks world

↑ **Parent:** [Classical planning](classical-planning.md)

The [blocks world](blocks-world.md) is a [classical planning](classical-planning.md) model of movable blocks arranged in stacks on an unlimited table. Each block has one support, each block supports at most one other block, and the support relation has no [directed cycle](directed-cycle.md). A clear block can move onto another clear block or onto the table. In a direct-transfer [STRIPS](strips.md) representation, an action includes the entire pickup-and-placement operation; a separate holding or empty-hand [planning fluent](planning-fluent.md) is unnecessary unless the action model explicitly splits those operations.

The table has unlimited capacity, so its availability must not be deleted when a block is placed there. [Planning state invariants](planning-state-invariant.md) connect the [predicate](predicate.md) describing a clear block to the absence of any block directly above it. [Goal interaction in planning](goal-interaction-in-planning.md) makes this small model useful for testing [automated planning](automated-planning.md) methods.

## ↑ Ancestors (5)

1. [Classical planning](classical-planning.md)
2. [Automated planning](automated-planning.md)
3. [Artificial intelligence](artificial-intelligence-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Blocks world](blocks-world.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/3/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/3/d/solution.md)
- [Sussman anomaly](sussman-anomaly.md)
