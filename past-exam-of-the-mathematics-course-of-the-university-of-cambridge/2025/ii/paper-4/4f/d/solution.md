<h1 id="4f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take

$$
G=(\{a,b,c\},\{S,A,B\},
\{S\to AB,\ A\to a,\ B\to b\},S)
$$

and

$$
G'=(\{a,b,c\},\{T\},\{T\to c\},T).
$$

These are variable based and have disjoint variable sets. They satisfy

$$
L(G)L(G')=\{abc\}.
$$

In $H^{\mathrm{reg}}$, however, both terminal productions of $G$ are replaced:

$$
A\to aT,\qquad B\to bT.
$$

Consequently its only terminal derivation is

$$
S\Rightarrow AB\Rightarrow aTB\Rightarrow aTbT
\Rightarrow acbc,
$$

so

$$
L(H^{\mathrm{reg}})=\{acbc\}\ne\{abc\}.
$$

This realizes the [failure of the regular concatenation construction for a nonregular grammar](../../../../../../failure-of-the-regular-concatenation-construction-for-a-nonregular-grammar.md): two different terminal productions introduce two copies of $T$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4F](../../4f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
