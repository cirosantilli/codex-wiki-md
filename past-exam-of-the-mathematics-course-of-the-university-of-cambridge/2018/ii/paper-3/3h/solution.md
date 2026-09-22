<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

The relation $g(X)h(X)=X^7-1$ makes this a length-seven binary [cyclic code](../../../../../cyclic-code.md). Since $\deg g=3$, the [generator polynomial of a cyclic code](../../../../../generator-polynomial-of-a-cyclic-code.md) gives

$$
\dim C=7-\deg g=4.
$$

The polynomial $g$ itself is a codeword of [Hamming weight](../../../../../hamming-weight.md) three, so the [minimum distance](../../../../../minimum-distance-of-a-code.md) is at most three. A nonzero word of weight one cannot vanish at the nonzero element $\alpha$. If a weight-two word $X^i+X^j$ vanished there, then $\alpha^{i-j}=1$; because $\alpha$ has order seven and $0\leq i,j<7$, this forces $i=j$. Hence there are no nonzero words of weight below three, and

$$
\boxed{\operatorname{rank}C=4,\qquad d(C)=3.}
$$

The equation $g(\alpha)=0$ gives $\alpha^3=\alpha^2+1$ in the [finite field](../../../../../finite-field.md) $\mathbb F_8$, and therefore

$$
\alpha^4=\alpha(\alpha^2+1)=\alpha^3+\alpha
=\alpha^2+\alpha+1=r(\alpha).
$$

By the [root-evaluation syndrome for a cyclic code](../../../../../root-evaluation-syndrome-for-a-cyclic-code.md), this is the syndrome of the single error $e(X)=X^4$. Since $d(C)=3$, [minimum-distance decoding](../../../../../minimum-distance-decoding.md) uniquely corrects one error. Subtracting and adding agree over $\mathbb F_2$, so the decoded codeword is

$$
\boxed{c(X)=r(X)+X^4=X^4+X^2+X+1=(X+1)g(X).}
$$

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
