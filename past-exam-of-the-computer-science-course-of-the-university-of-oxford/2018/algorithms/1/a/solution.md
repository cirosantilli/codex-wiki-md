<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [binary search tree](../../../../../binary-search-tree.md) is a [binary tree](../../../../../binary-tree.md) storing distinct keys from a [total order](../../../../../total-order.md), with every key in a node's left [subtree](../../../../../subtree.md) smaller than that node's key and every key in its right [subtree](../../../../../subtree.md) larger. The condition concerns entire [subtrees](../../../../../subtree.md), not just immediate neighbours.

For membership, start at the [root of a tree](../../../../../root-of-a-tree.md) and compare the target with the current key. **Return true on equality; continue into the left [subtree](../../../../../subtree.md) for a smaller target and the right [subtree](../../../../../subtree.md) for a larger target; return false on an empty [subtree](../../../../../subtree.md).** The [binary search tree](../../../../../binary-search-tree.md) ordering ensures that a discarded [subtree](../../../../../subtree.md) cannot contain the target. Each step descends one level, so the [algorithm](../../../../../algorithm-split.md) terminates and uses $O(h+1)$ [time complexity](../../../../../time-complexity.md) for [height of a binary tree](../../../../../height-of-a-binary-tree.md) $h$, under constant-time key comparison.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
