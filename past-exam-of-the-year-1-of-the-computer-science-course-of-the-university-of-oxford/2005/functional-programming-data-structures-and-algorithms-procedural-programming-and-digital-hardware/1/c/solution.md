<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [function extensionality](../../../../../function-extensionality.md): show $f(x)=g(x)$ for every value $x$ of the argument type. In [lazy evaluation](../../../../../lazy-evaluation.md) semantics, “every value” includes the [bottom value](../../../../../bottom-value.md) and partial values. For [list](../../../../../list-abstract-data-type.md) arguments, [structural induction on lazy lists](../../../../../structural-induction-on-lazy-lists.md) supplies the empty, bottom and cons cases, with continuity justifying passage to infinite [lists](../../../../../list-abstract-data-type.md).

The original printed equation has the same [right fold](../../../../../list-fold.md) on both sides, including the same operator and seed; this is visible in the scan.[Printed p. 2, Question 1(c), displayed equation](../../../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-examination-paper-by-the-university-of-oxford-2005.md) Thus its literal answer is

$$
\boxed{\operatorname{foldr}\ (\oplus)\ e=\operatorname{foldr}\ (\oplus)\ e
\quad\text{whenever the expression is well typed}.}
$$

For every input $xs$, both sides denote the very same expression `foldr (oplus) e xs`; equality follows by reflexivity. This remains true if its value is $\bot$. Neither termination nor [associativity](../../../../../associative-property.md) nor an identity law is required. The scan does not establish a different intended equation, so no replacement by a [left fold](../../../../../left-fold.md) is assumed.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
