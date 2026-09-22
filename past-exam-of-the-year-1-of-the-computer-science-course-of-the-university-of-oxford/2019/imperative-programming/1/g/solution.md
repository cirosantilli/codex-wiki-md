<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The first proposed identity can fail even without numerical error because [binary fractions](../../../../../binary-fraction.md) have nonunique textual representations. Leading zeroes, optional points and trailing fractional zeroes are normalized differently by a fixed-width output convention. It also fails if the input has more significant bits than `Double` can preserve, more fractional places than the output buffer can hold, an [integer](../../../../../integer-split.md) part outside the assumed `Int` range, or a value that overflows or underflows during decoding. [Array](../../../../../array-data-structure.md) identity here must mean equal contents: a newly allocated [Scala](../../../../../scala.md) [array](../../../../../array-data-structure.md) is a different [software object](../../../../../software-object.md), so use `sameElements` rather than reference equality for a content test.

The second identity fails when the stored fractional precision truncates a nonzero bit; **with two fractional places, $0.125$ becomes zero**. It can also fail outside the finite nonnegative input and [integer](../../../../../integer-split.md)-conversion assumptions. Within those assumptions, enough fractional positions to encode the finite `Double` exactly can permit the round trip, but an arbitrary fixed small width does not guarantee it. Every finite `Double` has a finite [binary expansion](../../../../../binary-expansion.md); saying that a decimal-looking `Double` necessarily has an infinite binary expansion would confuse the represented number with an exact decimal real.

The source's introductory example is internally inconsistent: the displayed digit [string](../../../../../string.md) has value $22+1/4+1/32=22.28125$, whereas its shortened character [array](../../../../../array-data-structure.md) encodes $22+1/4+1/16=22.3125$. The conversion rules above follow the actual input digits. **[Round-trip testing](../../../../../round-trip-testing.md) needs an independent value oracle as well as the two compositions**, because two mutually consistent but incorrect routines can conceal each other's errors.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
