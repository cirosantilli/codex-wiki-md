# Pareto efficiency of serial dictatorship with consecutive friends

↑ **Parent:** [Room allocation with friendship externalities](room-allocation-with-friendship-externalities.md)

Suppose each participant has at most one mutual friend, each friendship pair chooses consecutively, room values lie in $[0,1]$ and are distinct for each participant, and each friendship bonus exceeds $1$. Then every [subgame perfect equilibrium](subgame-perfect-equilibrium.md) outcome of [serial dictatorship](serial-dictatorship.md) is [Pareto optimal](pareto-efficiency.md).

For a friend pair, if any remaining adjacent room pair exists, the leader chooses their uniquely best room having an available neighbor; the follower chooses their uniquely best available neighbor. Adjacency dominates every possible difference in own-room value for both friends. If no adjacent room pair remains, neither friend can obtain a bonus and each chooses their unique best available room. A participant without a friend also chooses their unique best available room.

For the proof, compare a purported [Pareto improvement](pareto-improvement.md) block by block, where a block is a single participant without a friend or one consecutive friendship pair. Earlier fixed blocks leave the same rooms available. A block receiving adjacency cannot lose it in a weak improvement. Its leader must retain the uniquely best eligible room, and its follower must retain the uniquely best neighboring room. Without available adjacency, both rooms are fixed by strict own-room rankings. [Mathematical induction](mathematical-induction.md) fixes every assignment, excluding a strict improvement.

## ↑ Ancestors (8)

1. [Room allocation with friendship externalities](room-allocation-with-friendship-externalities.md)
2. [Serial dictatorship](serial-dictatorship.md)
3. [Mechanism design](mechanism-design.md)
4. [Game theory](game-theory-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/computational-game-theory/2/e/solution.md)
