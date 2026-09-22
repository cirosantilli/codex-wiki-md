<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Extract the two recorded parents from every matching certificate, and use [duplicate removal](../../../../../../duplicate-removal.md) so that repeated certificates do not repeat an individual. This helper is shared by the remaining [Haskell](../../../../../../haskell.md) definitions:

```
unique :: Eq a => [a] -> [a]
unique [] = []
unique (x:xs) = x : unique [y | y <- xs, y /= x]

parents :: Database -> Person -> [Person]
parents db p = unique [q | (baby,mother,father) <- db,
                          baby == p, q <- [mother,father]]
```

A person need not have a certificate of their own to appear in the output: a parental field is already evidence of the relationship. The resulting [list](../../../../../../list-abstract-data-type.md) preserves first occurrence order, with mother before father in each certificate. Its [set](../../../../../../set-split.md) of entries is

$$
\boxed{\{m\mid(p,m,f)\in db\}\cup\{f\mid(p,m,f)\in db\}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
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
