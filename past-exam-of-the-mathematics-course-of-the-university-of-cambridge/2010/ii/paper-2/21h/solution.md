<h1 id="21h/solution">Solution</h1>

↑ **Parent:** [21H](../21h.md)

Take a [CW complex](../../../../../cw-complex.md) with one vertex, loops labelled $a,b$, and one two-cell attached along $a^2b^3a^3b^2$. The [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) gives the required [fundamental group](../../../../../fundamental-group.md). Connected double [covering spaces](../../../../../covering-space.md) correspond to index-two subgroups, equivalently kernels of surjective homomorphisms $G\to C_2$. The relation imposes $5a+5b=0$ modulo two, so the unique nonzero possibility sends both $a,b$ to one. Thus **there is a unique connected double cover up to covering isomorphism.**

Construct it with two vertices; both labelled edges switch sheets, and attach the two lifts of the two-cell. Contract one of the $a$ edges to a spanning tree. With coset representatives $1,a$, the remaining [Schreier generators](../../../../../schreier-generator.md) can be taken as $A=a^2$, $B=ba^{-1}$ and $C=ab$. Reading the two lifts of the attaching word, starting on the two respective sheets, gives $ABCBA^2BC$ and $ACBCACB$. Thus

$$
\boxed{\pi_1(Y)=\langle A,B,C\mid ABCBA^2BC=1,\ ACBCACB=1\rangle}.
$$

For example, a letter $a$ contributes nothing on the first sheet and $A$ on the second; a letter $b$ contributes $B$ on the first and $C$ on the second. Both letters then switch sheets, which directly verifies the two relators.

## ↑ Ancestors (10)

1. [21H](../21h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
