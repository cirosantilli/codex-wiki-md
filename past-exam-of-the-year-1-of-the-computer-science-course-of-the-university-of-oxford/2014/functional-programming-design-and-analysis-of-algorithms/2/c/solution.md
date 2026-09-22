<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the first [binary relation](../../../../../binary-relation.md) for the outer generator, the second for the inner generator, and match their middle values. Different witnesses can generate the same output pair, so apply [duplicate removal](../../../../../duplicate-removal.md):

```
relcomp :: Eq a => [(a, a)] -> [(a, a)] -> [(a, a)]
relcomp r s = removedup [(a, b) | (a, c) <- r,
                                (d, b) <- s, c == d]
```

The guards give precisely the existential witness required for [composition of relations](../../../../../composition-of-relations.md):

$$
\boxed{(a,b)\in\operatorname{relcomp}(R,S)\iff\exists c:\ (a,c)\in R\ \land\ (c,b)\in S.}
$$

Every output is sound by its generating witness, and every witness is visited for finite inputs. [Duplicate removal](../../../../../duplicate-removal.md) converts the resulting enumeration back to the required representation by distinct pairs.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
