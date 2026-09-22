<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use one-based row numbers, and write $F$ and $L$ for the first and last columns. The [last-to-first mapping](../../../../../last-to-first-mapping.md) matches the $k$th occurrence of a character in $L$ to its $k$th occurrence in $F$: equal characters retain the ordering of their following suffixes. This lets us extend an interval of matching [suffixes](../../../../../string-suffix.md) one character to the left without reconstructing the full strings.

Start with the last query character. Rows $5,6,7$ of $F$ contain C, so the interval of [suffixes](../../../../../string-suffix.md) beginning with C is $[5,7]$. Within those rows, the A entries of $L$ are at rows $5$ and $7$. They are respectively the first and second A entries in all of $L$, and therefore map to rows $2$ and $3$ of $F$. These are exactly the [suffixes](../../../../../string-suffix.md) beginning with AC. Reading their supplied positions gives **matches starting at positions 11 and 3**, or positions **3 and 11** in increasing genomic order.

The same calculation can be written as [backward search](../../../../../backward-search.md). Let $C(c)$ count characters strictly smaller than $c$, and let $\operatorname{Occ}(c,r)$ count occurrences of $c$ in $L[1:r]$, with $\operatorname{Occ}(c,0)=0$. Prepending $c$ changes an inclusive interval $[l,r]$ to

$$
[l',r']=[C(c)+\operatorname{Occ}(c,l-1)+1,\ C(c)+\operatorname{Occ}(c,r)].
$$

Here $C(\mathrm A)=1$, $\operatorname{Occ}(\mathrm A,4)=0$ and $\operatorname{Occ}(\mathrm A,7)=2$, giving $[l',r']=[2,3]$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
