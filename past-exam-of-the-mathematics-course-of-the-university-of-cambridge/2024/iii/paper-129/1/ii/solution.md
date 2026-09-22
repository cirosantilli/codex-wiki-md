<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Construct $X\subseteq B$ greedily. Begin with one element of $B$. While some $b\in B$ satisfies

$$
|(A+b)\cap(A+X)|\le |A|/2,
$$

adjoin $b$ to $X$. The first translate contributes $|A|$ points to $A+X$, and each later translate contributes at least $|A|/2$ new points. Therefore

$$
|A+B|\ge|A+X|\ge |A|+(|X|-1)|A|/2,
$$

and hence

$$
\boxed{|X|\le 2|A+B|/|A|-1.}
$$

When the process stops, every $b\in B$ satisfies $|(A+b)\cap(A+X)|>|A|/2$. Each point in this intersection has the form

$$
b+a'=x+a,
$$

and therefore gives a triple $(x,a,a')\in X\times A\times A$ with $b=a-a'+x$. Distinct intersection points give distinct $a'$, so there are more than $|A|/2$ such triples.

For $b,b'\in B$, the corresponding sets of possible $a'\in A$ both have size greater than $|A|/2$ and hence intersect. Using a common $a'$ gives

$$
b=a-a'+x,
\qquad
b'=c-a'+y,
$$

so $b-b'=a-c+x-y$. Thus

$$
\boxed{B-B\subseteq A-A+X-X.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
