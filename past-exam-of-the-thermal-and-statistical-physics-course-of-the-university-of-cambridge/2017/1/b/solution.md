<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Repeated letters.** There are six positions, with two copies of each of two letters. Counting labeled arrangements and dividing by the [permutations](../../../../permutation.md) of each repeated pair gives

$$
\boxed{\frac{6!}{2!\,2!}=180.}
$$

**Single-occupancy cells.** For $N$ indistinguishable particles, specifying which $N$ of the $M$ distinct cells are occupied completely specifies a configuration. Thus

$$
\boxed{W_{\rm indist}=\binom MN=\frac{M!}{N!(M-N)!}.}
$$

For distinguishable particles, each chosen occupied set admits $N!$ assignments of particle labels:

$$
\boxed{W_{\rm dist}=\binom MN N!=\frac{M!}{(M-N)!}.}
$$

Equivalently, successively place labeled particles in $M,M-1,\ldots,M-N+1$ available cells. The single-occupancy constraint is essential: this is not unrestricted [stars and bars](../../../../stars-and-bars-combinatorics.md). Both counts give one empty configuration at $N=0$; at $N=M$ they give one unlabeled occupation pattern and $M!$ labeled assignments.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
