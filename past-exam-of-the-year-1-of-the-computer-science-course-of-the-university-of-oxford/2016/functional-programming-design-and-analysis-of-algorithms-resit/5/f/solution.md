<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The displayed procedure calls `Find-Set` **$2|E|$ times explicitly**, since it tests the two endpoints of every edge. Each successful `Union` decreases the number of sets by one, from $|V|$ initially to $k$ finally, so **there are $|V|-k$ `Union` calls**.

These are calls at the displayed pseudocode level. If a concrete `Union(u,v)` implementation performs two further internal finds rather than accepting already found roots, its implementation adds $2(|V|-k)$ find invocations. Counting those separately avoids confusing the procedure's explicit call count with the implementation of a [disjoint-set union operation](../../../../../disjoint-set-union-operation.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
