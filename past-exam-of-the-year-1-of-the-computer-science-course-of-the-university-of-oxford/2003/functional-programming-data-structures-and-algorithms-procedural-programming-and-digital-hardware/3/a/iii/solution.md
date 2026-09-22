<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Treat brothers as male individuals sharing at least one recorded parent, including half-brothers. Derive a sibling helper and then select the recorded sex:

```
siblings :: Database -> Person -> [Person]
siblings db p = unique [q | parent <- parents db p,
                           q <- children db parent, q /= p]

brothers :: Database -> Person -> [Person]
brothers db p = [q | q <- siblings db p, sex q == Male]
```

The exclusion `q /= p` prevents a male individual from being his own brother. [Duplicate removal](../../../../../../duplicate-removal.md) is needed because a full brother can be found through both parents. The membership condition is

$$
\boxed{q\ne p,\quad\operatorname{sex}(q)=\mathrm{Male},\quad
\operatorname{parents}(db,q)\cap\operatorname{parents}(db,p)\ne\varnothing.}
$$

If the intended convention is _full_ brothers only, replace the shared-parent condition by a common mother and a common father in the recorded certificates. The definition above states the convention explicitly rather than silently discarding half-brothers.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
