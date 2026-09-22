# Null child slot count

↑ **Parent:** [Binary tree child slot](binary-tree-child-slot.md)

Every nonempty finite [binary tree](binary-tree.md) with $n$ [vertices](vertex-graph-theory.md) has exactly $n+1$ empty [binary tree child slots](binary-tree-child-slot.md). There are $2n$ slots altogether, and precisely $n-1$ occupied slots, one for each [edge](edge-of-a-graph.md) of its underlying [tree](tree-graph-theory-split.md). Therefore

$$
2n-(n-1)=n+1.
$$

This counts missing child references, not [vertices](vertex-graph-theory.md) or leaves. In the mixed four-[vertex](vertex-graph-theory.md) example, $A$ has no empty [binary tree child slots](binary-tree-child-slot.md), $B$ has one, and $C,D$ each have two: $0+1+2+2=5$. The four-[vertex](vertex-graph-theory.md) chain also has five: one at each of its first three [vertices](vertex-graph-theory.md) and two at the last. For $n=0$, there are no [vertices](vertex-graph-theory.md) and hence no child fields; the empty [binary tree](binary-tree.md) instead has a single empty root position if it is represented by a root reference.

A second proof uses the recursive decomposition. Count every empty [subtree](subtree.md) occurrence, including the root position for the empty [binary tree](binary-tree.md): let $e(\varnothing)=1$. For a nonempty [binary tree](binary-tree.md), $e(T)=e(L)+e(R)$. If the two [subtrees](subtree.md) have $n_L,n_R$ [vertices](vertex-graph-theory.md), [structural induction](structural-induction.md) gives $e(T)=(n_L+1)+(n_R+1)=n+1$. Distinct empty positions may share the same `null` value; these are occurrences, not separately allocated objects. This count is useful when analysing the base cases reached by a [structural recursion](structural-recursion.md) that calls both [subtrees](subtree.md) of every [vertex](vertex-graph-theory.md).

## ↑ Ancestors (5)

1. [Binary tree child slot](binary-tree-child-slot.md)
2. [Binary tree](binary-tree.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
