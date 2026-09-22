<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Center the board at the origin and map each white square $(i,j)$ to

$$
(u,v)=\left(\frac{i+j}{2},\frac{i-j}{2}\right).
$$

The white squares become the integer points of the diamond

$$
D_n=\{(u,v)\in\mathbb Z^2:|u|+|v|\leq n\},
$$

and a bishop move changes exactly one coordinate. From $(u,v)$ the chain can move first to $(u,0)$ and then to $(0,0)$, since both points lie in $D_n$. Reversing such paths connects any two states, so the [bishop random walk](../../../../../../bishop-random-walk.md) is an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
