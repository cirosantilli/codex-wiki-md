<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Enumerate by the hypotenuse and test finitely many shorter legs:
```
primitiveTriples :: [(Integer, Integer, Integer)]
primitiveTriples =
  [(a, b, c) |
     c <- [1..],
     b <- [1..c-1],
     a <- [1..b-1],
     a*a + b*b == c*c,
     gcd a (gcd b c) == 1]
```
The equality selects [Pythagorean triples](../../../../../pythagorean-triple.md), and the [greatest common divisor](../../../../../greatest-common-divisor.md) test makes them primitive. The bounds enforce $0<a<b<c$, removing the duplicate obtained by exchanging the legs. Each fixed $c$ has a finite search, so the outer loop gives ascending hypotenuse order and reaches every qualifying triple. Infinite families supplied by [Euclid's formula](../../../../../euclid-s-formula-for-pythagorean-triples.md) ensure that the stream has arbitrarily many outputs. Its first five entries are
```
[(3,4,5),(5,12,13),(8,15,17),(7,24,25),(20,21,29)]
```
Using `Integer` avoids overflow in the squared values. The construction prioritizes a direct correctness argument; it does not claim an optimal enumeration cost.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
