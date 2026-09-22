<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A matching mother or father field identifies a child. In [Haskell](../../../../../../haskell.md):

```
children :: Database -> Person -> [Person]
children db p = unique [baby | (baby,mother,father) <- db,
                              mother == p || father == p]
```

[Duplicate removal](../../../../../../duplicate-removal.md) handles repeated certificates and children recorded in more than one matching row. Thus

$$
\boxed{\operatorname{children}(db,p)=\{c\mid(c,m,f)\in db,\ m=p\ \lor\ f=p\}.}
$$

The displayed [set](../../../../../../set-split.md) describes membership; the implementation returns its entries as a [list](../../../../../../list-abstract-data-type.md) in first certificate order.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
