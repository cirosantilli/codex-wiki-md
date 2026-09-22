<h1 id="3/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use first cousins: the children of the siblings of a recorded parent. This includes cousins through a parent's half-sibling under the convention above. In [Haskell](../../../../../../haskell.md):

```
cousins :: Database -> Person -> [Person]
cousins db p = unique [q | parent <- parents db p,
                          auntOrUncle <- siblings db parent,
                          q <- children db auntOrUncle, q /= p]
```

Selecting siblings of parents avoids the mistake of returning all people with a common grandparent, which would also return ordinary siblings. The explicit exclusion of `p` is harmless on an ordinary consistent pedigree and prevents a self-result in unusual records. Multiple relationship paths give just one output entry after [duplicate removal](../../../../../../duplicate-removal.md). Thus

$$
\boxed{\operatorname{cousins}(db,p)=
\bigcup_{r\in\operatorname{parents}(db,p)}\ \bigcup_{s\in\operatorname{siblings}(db,r)}
\operatorname{children}(db,s)\setminus\{p\}.}
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
