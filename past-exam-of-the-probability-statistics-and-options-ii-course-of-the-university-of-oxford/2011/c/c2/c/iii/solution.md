<h1 id="c/c2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An integer square is a square modulo every prime, with the zero class allowed at primes dividing the integer. Conversely, suppose an odd integer $a$ is not an integer square. If every prime exponent in $|a|$ is even, the nonsquare condition forces $a=-b^2$, handled by part (i). Otherwise some odd prime has an odd exponent, so $a=\pm q^tb$ as in part (ii). In either case there is a positive odd $k$ with $(a/k)=-1$.

Factor $k$ into odd primes. A product of Legendre symbols equalling minus one has at least one factor equal to minus one. Thus $a$ fails to be a square modulo one of those primes, contradicting the hypothesis. Hence

$$
\boxed{a\in\mathbb Z\text{ odd is an integer square iff }x^2\equiv a\pmod p\text{ is solvable for every prime }p.}
$$

The solvability formulation makes explicit the zero-residue convention needed by the printed final assertion. The prime two causes no extra issue because every odd integer is one modulo two.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [C2](../../../c2.md)
4. [C](../../../../c.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
