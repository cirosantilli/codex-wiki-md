<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [trie](../../../../../trie.md) node needs a terminal flag as well as its children: a stored word can also be the prefix of a longer stored word.
```
TYPE Trie = POINTER TO Node;
     Node = RECORD
       terminal: BOOLEAN;
       child: ARRAY 26 OF Trie
     END;
```
Index zero denotes `a`, index 25 denotes `z`; [null pointers](../../../../../null-pointer.md) denote absent branches. The [set](../../../../../set-split.md) represented by a nonnull node consists of the empty [string](../../../../../string.md) if `terminal` is true, together with every child's words prefixed by that child's letter. **Represent the empty [set](../../../../../set-split.md) by `NIL`.** The singleton containing the empty [string](../../../../../string.md) instead has a terminal root and no children.

**The declarations alone do not force a unique representation.** A nonterminal leaf, or a whole branch without terminal descendants, contributes no word. To obtain uniqueness up to pointer addresses, impose a [representation invariant](../../../../../representation-invariant.md): the structure is a finite [rooted tree](../../../../../rooted-tree.md), and each allocated node lies on a path to a terminal node. Then precisely the prefixes of stored words exist, all flags are determined, and the empty [set](../../../../../set-split.md) has only the `NIL` representation. The insertion procedures below preserve this invariant when starting with such a [trie](../../../../../trie.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
