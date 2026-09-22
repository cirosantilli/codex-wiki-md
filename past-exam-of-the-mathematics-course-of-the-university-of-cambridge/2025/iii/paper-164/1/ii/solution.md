<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $S_1=H(X)+H(Y)+H(Z)$ and $S_2=H(X,Y)+H(Y,Z)+H(Z,X)$. By the definition of [mutual information](../../../../../../mutual-information.md),

$$
I(X;Y)+I(Y;Z)+I(Z;X)=2S_1-S_2,
$$

so the required right-hand side is $(2S_2-S_1)/3$.

Apply [entropy submodularity](../../../../../../entropy-submodularity.md) to the pairs $(X,Y),(X,Z)$ and then cyclically permute the variables:

$$
\begin{aligned}
H(X,Y)+H(X,Z)&\geq H(X)+H(X,Y,Z),\\
H(Y,Z)+H(Y,X)&\geq H(Y)+H(X,Y,Z),\\
H(Z,X)+H(Z,Y)&\geq H(Z)+H(X,Y,Z).
\end{aligned}
$$

Adding gives $2S_2\geq S_1+3H(X,Y,Z)$, which is exactly

$$
\boxed{H(X,Y,Z)\leq\frac12S_2-\frac16(2S_1-S_2).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
