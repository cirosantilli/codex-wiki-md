<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose a circular [doubly linked list](../../../../../doubly-linked-list.md) with a permanent dummy [list header](../../../../../list-header.md). For a concrete [Oberon](../../../../../oberon-programming-language.md) definition take `data = INTEGER`; the same link operations work with any chosen data [data type](../../../../../data-type.md):

```
TYPE data = INTEGER;
     pointerToNode = POINTER TO node;
     node = RECORD
       value : data;
       prev, next : pointerToNode
     END;

PROCEDURE NewList() : pointerToNode;
VAR h : pointerToNode;
BEGIN
  NEW(h);
  h.prev := h;
  h.next := h;
  RETURN h
END NewList;

PROCEDURE Insert(v : data; n : pointerToNode);
VAR t, p : pointerToNode;
BEGIN
  p := n.prev;
  NEW(t);
  t.value := v;
  t.prev := p;
  t.next := n;
  p.next := t;
  n.prev := t
END Insert;

PROCEDURE Delete(n : pointerToNode);
VAR p, q : pointerToNode;
BEGIN
  p := n.prev;
  q := n.next;
  p.next := q;
  q.prev := p;
  n.prev := NIL;
  n.next := NIL
END Delete;
```

The representation invariant is that the live nodes and header form one finite circular chain, with every neighboring next/previous pair mutually consistent. `Insert` replaces the link $p\leftrightarrow n$ by $p\leftrightarrow t\leftrightarrow n$. `Delete` replaces $p\leftrightarrow n\leftrightarrow q$ by $p\leftrightarrow q$. All other links remain unchanged. These arguments also cover insertion into an empty [linked list](../../../../../linked-list.md) and deletion of its sole data node, where the neighboring positions can refer to the same header.

`Insert` requires a live node `n` belonging to this representation and successful allocation. It may be called with `n` equal to the header, meaning append just before the end. `Delete` requires a live _data_ node and must never be called on the header, on `NIL`, or on a node already deleted or belonging to an incompatible representation. The signature alone cannot enforce those [preconditions](../../../../../precondition.md). The detached node is left for [garbage collection](../../../../../garbage-collection.md); external references must no longer treat it as a member of the [linked list](../../../../../linked-list.md). Neither update contains a loop. Apart from allocation and memory management, the link work is

$$
\boxed{O(1)\text{ for insertion before a known node and deletion of a known data node}.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
