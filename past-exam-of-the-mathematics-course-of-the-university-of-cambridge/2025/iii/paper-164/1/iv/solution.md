<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For random variables $A,B$ in a [finite additive group](../../../../../../finite-additive-group.md), take independent copies $A',B'$ with the same respective distributions and define the [Entropic Ruzsa distance](../../../../../../entropic-ruzsa-distance.md) by

$$
d_R(A,B)=H(A'-B')-\frac12H(A')-\frac12H(B').
$$

For the independent variables in the question, expansion gives

$$
d_R(X,Z)+d_R(Y,Z)-d_R(X,Y)
=H(X-Z)+H(Y-Z)-H(X-Y)-H(Z).
$$

Part iii, applied to the independent variables $X,Y,-Z$, says

$$
H(X+Y-Z)+H(Z)\leq H(X-Z)+H(Y-Z).
$$

Subtracting $H(X-Y)$ from both sides proves

$$
H(X+Y-Z)-H(X-Y)
\leq d_R(X,Z)+d_R(Y,Z)-d_R(X,Y).
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 164](../../../paper-164-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
